# BUG-004 — Descending elevator pushes the player below the playable map

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

- The player has access to the elevator.

## Steps to Reproduce

1. Position the player underneath the elevator platform.
2. Activate or call the elevator so that the platform descends.
3. Remain underneath the descending platform.

## Actual Result

The elevator pushes the player through the environment and underneath the playable map.

## Expected Result

The elevator should prevent the player from entering invalid geometry, for example by blocking access or moving the player to a safe position.

## Evidence

Video recording available.

## Notes

- The behavior can also be reproduced while riding the motorcycle.
- The player can return to the playable area, so the issue does not create a permanent softlock.
- Normal elevator usage works correctly.
