

https://github.com/user-attachments/assets/10c37bd9-9942-460a-a47b-906ff908c342

# BUG-003 — Invalid two-tool state allows the player to launch above the map

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

- [BUG-002](BUG-002-Two-Tools-Simultaneously.md) has been reproduced.
- The player possesses both the baseball bat and blower simultaneously.

## Steps to Reproduce

1. Obtain both tools by following the steps in BUG-002.
2. Look downward.
3. Hold `S`.
4. Repeatedly use the tools underneath or near the player.
5. Continue the interaction.

## Actual Result

The player gains repeated upward displacement and can eventually move above the intended playable area.

## Expected Result

Tool physics should not allow the player to generate unlimited upward movement or leave the playable boundaries.

## Evidence

https://github.com/user-attachments/assets/755dc753-7770-46e2-bb06-ee0666843303

## Related Issues

- [BUG-002 — Player can obtain two tools during elevator descent](BUG-002-Two-Tools-Simultaneously.md)

## Notes

A comparison test confirmed that the baseball bat alone does not create unlimited upward movement.
https://github.com/user-attachments/assets/e9723ddf-5667-4532-982e-22b47db97b2f

