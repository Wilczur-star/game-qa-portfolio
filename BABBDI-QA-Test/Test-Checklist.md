# BABBDI Executed Test Checklist

## Status Key

- **PASS** — observed behavior matched the expected result.
- **FAIL** — a reproducible defect was confirmed.
- **OBSERVATION** — behavior was recorded, but design intent requires verification.

## Executed Checks

| ID | Test | Expected Result | Status | Notes |
| --- | --- | --- | --- | --- |
| CHK-001 | Launch and restart the game | Game launches and restarts correctly | PASS | No issue observed |
| CHK-002 | Change the master volume and revisit the setting | Audio level changes and the selected value persists | PASS | No issue observed |
| CHK-003 | Change graphics quality and revisit the setting | Quality changes and the selected value persists | PASS | No issue observed |
| CHK-004 | Use Alt+Tab during play | Game continues to operate normally | PASS | No issue observed |
| CHK-005 | Walk, sprint, jump, and crouch | Basic movement responds correctly | PASS | Movement also felt smooth |
| CHK-006 | Use the elevator normally | Elevator transports the player without an issue | PASS | Normal use worked correctly |
| CHK-007 | Attempt normal movement while riding the elevator | Normal player movement is restricted during the ride | PASS | Restriction worked as expected |
| CHK-008 | Attempt to collect a second tool during normal play | One-tool restriction remains enforced | PASS | Two tools could not simply be picked up normally |
| CHK-009 | Use the baseball bat alone for repeated upward movement | Bat alone does not provide unlimited upward movement | PASS | Used as a comparison for BUG-003 |
| CHK-010 | Press the key shown in the NPC interaction prompt | Displayed key starts the conversation | FAIL | Prompt shows `X`; `E` starts dialogue — [BUG-001](Bug-Reports/BUG-001-Incorrect-Interaction-Key.md) |
| CHK-011 | Pick up the blower during elevator descent while holding the bat | One-tool restriction remains enforced | FAIL | Player obtains both tools — [BUG-002](Bug-Reports/BUG-002-Two-Tools-Simultaneously.md) |
| CHK-012 | Use both tools while looking down and moving backward | Tool use does not create unlimited vertical movement | FAIL | Player can launch above the map — [BUG-003](Bug-Reports/BUG-003-Player-Launch-Above-Map.md) |
| CHK-013 | Remain underneath the descending elevator | Player stays within playable geometry | FAIL | Player is pushed below the map — [BUG-004](Bug-Reports/BUG-004-Elevator-Clips-Player-Out-Of-Bounds.md) |
| CHK-014 | Interact twice with the starting-area NPC | Introduction precedes later farewell dialogue | FAIL | Dialogue order is reversed — [BUG-005](Bug-Reports/BUG-005-Incorrect-Dialogue-Order.md) |
| CHK-015 | Throw the baseball bat toward solid level geometry | Tool remains accessible or returns to a valid position | FAIL | Bat becomes inaccessible until the save is reset — [BUG-006](Bug-Reports/BUG-006-Bat-Lost-In-Geometry.md) |
| CHK-016 | Observe NPC head tracking during interaction | Rotation remains visually plausible | OBSERVATION | Approximately 180° rotation; design intent is uncertain — [OBS-001](Observations/OBS-001-NPC-Head-Rotation.md) |
| CHK-017 | Use a window near the starting area to bypass part of the route | Route boundaries behave as intended | OBSERVATION | The route can be bypassed and the player can return; intentionality was not established |

## Summary

| Result | Count |
| --- | ---: |
| PASS | 9 |
| FAIL | 6 |
| OBSERVATION | 2 |
| **Total** | **17** |

The second observation was not filed as a defect because the intended route boundaries were not known.
