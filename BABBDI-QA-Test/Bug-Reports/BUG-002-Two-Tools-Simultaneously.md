# BUG-002 — Player can obtain two tools during elevator descent

| Field | Value |
| --- | --- |
| Status | Confirmed |
| Severity | Major |
| Priority | High |
| Reproducibility | 100% |

## Environment

- Windows 11
- PC
- Keyboard and mouse

## Preconditions

- The player has access to the baseball bat, blower, and elevator.

## Steps to Reproduce

1. Pick up the baseball bat.
2. Go to the location containing the blower.
3. Call the elevator.
4. Pick up the blower.
5. Throw or drop the blower inside the elevator.
6. Pick up the baseball bat again.
7. Enter the elevator.
8. Activate the elevator.
9. During the descent, wait until the blower remains above the player's head because it falls more slowly than the elevator.
10. Press `E` while the blower is within interaction range.

## Actual Result

The player picks up the blower while retaining the baseball bat and possesses two tools simultaneously.

## Expected Result

The normal one-tool limit should remain enforced. The game should prevent the pickup or replace/drop the currently held tool.

## Evidence

Video recording available.

## Related Issues

- [BUG-003 — Two-tool state allows the player to launch above the map](BUG-003-Player-Launch-Above-Map.md)

## Notes

Normal gameplay does not allow the player to simply pick up two tools. The issue depends on the interaction between item physics and the descending elevator.
