# BUG-001 — Interaction prompt displays the wrong key

| Field | Value |
| --- | --- |
| Status | Confirmed |
| Severity | Medium |
| Priority | High |
| Reproducibility | 100% |

## Environment

- Windows 11
- PC
- Keyboard and mouse

## Preconditions

- The player is able to approach and interact with the affected NPC.

## Steps to Reproduce

1. Approach the affected NPC.
2. Observe the `TALK [X]` interaction prompt.
3. Press `X`.
4. Press `E`.

## Actual Result

Pressing `X` does not start the conversation. Pressing `E` starts it.

## Expected Result

The key displayed in the interaction prompt should start the conversation, or the prompt should display the actual interaction key.

## Evidence

Video recording available.
