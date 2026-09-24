# BABBDI Exploratory Test Session Report

## Session Summary

| Field | Result |
| --- | --- |
| Session type | Exploratory manual testing |
| Duration | Approximately 20–30 minutes |
| Environment | Windows 11, PC, keyboard and mouse |
| Confirmed defects | 6 |
| Visual observations filed | 1 |

## Session Goal

Explore selected gameplay systems under both normal and unusual player behavior, verify discovered issues, and produce concise reports that another tester or developer could follow.

## Areas Tested

- Launch and restart behavior
- Selected audio and graphics settings
- Alt+Tab behavior
- Basic movement
- NPC interaction prompts and dialogue sequence
- Tool pickup and use
- Elevator operation
- Physics and collision edge cases
- Out-of-bounds and item-recovery behavior
- Visual NPC behavior

## Passed Checks

- The game launched and restarted correctly.
- Master volume worked and persisted.
- Graphics quality worked and persisted.
- Alt+Tab worked normally.
- Walking, sprinting, jumping, and crouching worked correctly.
- Movement felt smooth during the session.
- Normal elevator usage worked correctly.
- The game disabled normal player movement while riding the elevator.
- Normal gameplay did not allow the player to simply pick up two tools at once.
- The baseball bat alone did not allow unlimited upward movement.

## Confirmed Defects

| ID | Finding | Severity | Priority |
| --- | --- | --- | --- |
| [BUG-001](Bug-Reports/BUG-001-Incorrect-Interaction-Key.md) | Incorrect interaction key displayed | Medium | High |
| [BUG-002](Bug-Reports/BUG-002-Two-Tools-Simultaneously.md) | Two tools can be held simultaneously | Major | High |
| [BUG-003](Bug-Reports/BUG-003-Player-Launch-Above-Map.md) | Two-tool state enables launch above the map | Major | High |
| [BUG-004](Bug-Reports/BUG-004-Elevator-Clips-Player-Out-Of-Bounds.md) | Elevator pushes the player below the map | Major | High |
| [BUG-005](Bug-Reports/BUG-005-Incorrect-Dialogue-Order.md) | NPC dialogue plays in the wrong order | Medium | Medium |
| [BUG-006](Bug-Reports/BUG-006-Bat-Lost-In-Geometry.md) | Baseball bat becomes inaccessible in geometry | Medium | Medium |

## Defect Relationship

BUG-002 creates an invalid inventory state in which the player possesses both the baseball bat and blower. That state is a precondition for BUG-003, which allows the player to gain excessive vertical movement and leave the intended play area. A comparison test confirmed that the baseball bat alone does not produce unlimited upward movement.

## Observations

- [OBS-001](Observations/OBS-001-NPC-Head-Rotation.md): an NPC's head can rotate to a visually unnatural angle of approximately 180°. Because the game's visual style may make this intentional, it remains an observation rather than a confirmed defect.
- A window near the starting area can bypass part of the intended route. The player can return, and the intended design was not established, so no bug was filed.

## Recovery Findings

- The player can return to the playable area after being pushed below the map by the elevator; the issue is not a permanent softlock.
- The inaccessible baseball bat returns only after the save is reset or restarted.

## Evidence

Video recordings are available for the reported findings.

## Limitations

This was a short, focused session rather than a full test pass. The game version, exact test date, hardware configuration, performance metrics, controller behavior, and complete game coverage were not recorded. No result outside the documented session has been inferred.

## Conclusion

The session confirmed that the tested core controls and selected settings behaved correctly, while physics, collision boundaries, interaction feedback, and dialogue sequencing produced reproducible issues. The highest-risk findings involve leaving the playable area and chaining an invalid inventory state into a second movement exploit.
