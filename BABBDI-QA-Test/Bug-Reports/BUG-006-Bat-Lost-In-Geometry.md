# BUG-006 — Baseball bat becomes inaccessible inside level geometry

| Field | Value |
| --- | --- |
| Status | Confirmed |
| Severity | Medium |
| Priority | Medium |
| Reproducibility | 100% |

## Environment

- Windows 11
- PC
- Keyboard and mouse

## Preconditions

- The player has obtained the baseball bat.

## Steps to Reproduce

1. Stand close to a wall or other solid level geometry.
2. Throw or drop the baseball bat toward the geometry.
3. Allow the bat to pass inside or beyond the playable geometry.
4. Attempt to retrieve it.

## Actual Result

The baseball bat becomes inaccessible and cannot be recovered during the current run.

## Expected Result

The tool should remain within reachable space or be repositioned to a valid location after entering inaccessible geometry.

## Evidence

Video recording available.

## Notes

Resetting or restarting the save makes the baseball bat available again. Without that recovery action, it remains lost for the current run.
