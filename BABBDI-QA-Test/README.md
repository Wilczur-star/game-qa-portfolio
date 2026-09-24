# BABBDI QA Test

This project documents a focused exploratory testing session of **BABBDI**. The goal was to examine core controls and settings, interactions, item handling, elevator behavior, collision boundaries, NPC dialogue, and unusual player actions.

## Why this game?

Game was suggested by AI as I didn't wanted to test games that I know very well and testing indie game has higher possibilities to find bugs quicker. Tho in this type of games, bugs often become a "feature" especially for speedruners.
That being said, I have never heard of the game before, I didn't see any video or image of the gameplay before playing it by myself and all bugs written out here are found by myself. Seeing how easly I managed to get those bugs I expected them to be popular/well-known already.

## Test Overview

| Item | Details |
| --- | --- |
| Test type | Exploratory manual testing |
| Session duration | Approximately 20–30 minutes |
| Platform | PC |
| Operating system | Windows 11 |
| Input | Keyboard and mouse |
| Confirmed defects | 6 |
| Additional observations | 1 visual observation requiring further verification |

## Results at a Glance

| ID | Summary | Severity | Priority | Result |
| --- | --- | --- | --- | --- |
| [BUG-001](Bug-Reports/BUG-001-Incorrect-Interaction-Key.md) | Interaction prompt shows `X`, but dialogue starts with `E` | Medium | High | Confirmed |
| [BUG-002](Bug-Reports/BUG-002-Two-Tools-Simultaneously.md) | Elevator descent allows the player to obtain two tools simultaneously | Major | High | Confirmed |
| [BUG-003](Bug-Reports/BUG-003-Player-Launch-Above-Map.md) | Invalid two-tool state can launch the player above the map | Major | High | Confirmed |
| [BUG-004](Bug-Reports/BUG-004-Elevator-Clips-Player-Out-Of-Bounds.md) | Descending elevator pushes the player below the playable map | Major | High | Confirmed |
| [BUG-005](Bug-Reports/BUG-005-Incorrect-Dialogue-Order.md) | NPC greeting and farewell dialogue play in the wrong order | Medium | Medium | Confirmed |
| [BUG-006](Bug-Reports/BUG-006-Bat-Lost-In-Geometry.md) | Baseball bat becomes inaccessible after entering level geometry | Medium | Medium | Confirmed |
| [OBS-001](Observations/OBS-001-NPC-Head-Rotation.md) | NPC head rotates to a visually unnatural angle | Low / Observation | — | Further verification required |

## Project Documents

- [Test Plan](Test-Plan.md)
- [Executed Test Checklist](Test-Checklist.md)
- [Test Session Report](Test-Session-Report.md)
- [Bug Reports](Bug-Reports/)
- [Observations](Observations/)

The reports distinguish confirmed defects from behavior that may be intentional. Game version 1.2.5. No hardware specification, or other unrecorded test data has been added.
