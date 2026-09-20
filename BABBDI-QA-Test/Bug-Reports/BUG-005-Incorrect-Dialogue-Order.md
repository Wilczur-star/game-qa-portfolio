# BUG-005 — NPC dialogue lines play in the wrong order

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

- Start from a fresh or reset save.

## Steps to Reproduce

1. Start a new game.
2. Approach the affected NPC near the starting area.
3. Interact with the NPC for the first time.
4. Finish the dialogue.
5. Interact with the same NPC again.

## Actual Result

The NPC uses a farewell-type line during the first interaction. The greeting/introduction and information about taking the baseball bat appear during the second interaction.

## Expected Result

The introductory dialogue should appear during the first interaction, followed by the appropriate later dialogue during subsequent interactions.

## Evidence

Video recording available.

## Notes

The issue was reproduced multiple times, including after a fresh start.
