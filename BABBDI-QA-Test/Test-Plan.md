# BABBDI Test Plan

## Objective

Evaluate the stability and behavior of selected BABBDI systems during normal play and unusual player actions, then document reproducible defects in a clear format.

## Test Approach

- Short exploratory manual test session
- Positive checks of expected behavior
- Negative and edge-case testing around physics and collision boundaries
- Reproduction of discovered issues
- Comparison tests to isolate relevant conditions
- Recovery checks where the player or an item entered an invalid state

## Test Environment

| Field | Value |
| --- | --- |
| Operating system | Windows 11 |
| Platform | PC |
| Input method | Keyboard and mouse |

The game version and hardware specifications were not recorded.

## In Scope

- Game launch and restart
- Master volume and graphics-quality settings
- Alt+Tab behavior
- Basic movement: walking, sprinting, jumping, and crouching
- NPC interaction prompts and dialogue order
- Tool pickup, use, and disposal
- Normal and unusual elevator interaction
- Player and item collision with level geometry
- Recovery from out-of-bounds or inaccessible-item states
- Visual NPC behavior encountered during the session

## Areas of Focus

1. Verify that core controls and selected settings work and persist.
2. Compare normal tool behavior with unusual physics interactions.
3. Test the elevator during normal use and while the player is in unsafe positions.
4. Explore whether items or the player can enter inaccessible geometry.
5. Repeat discovered issues to establish reproducibility.
6. Record uncertain visual behavior separately from confirmed defects.

## Evidence

Video recordings were captured for the reported findings. Media files are not included in this repository.

## Limitations

- The session lasted approximately 20–30 minutes.
- Testing was limited to the recorded environment and selected gameplay areas.
- No performance measurements, hardware matrix, controller testing, or full-game coverage were recorded.
- Behaviors with uncertain design intent were not classified as confirmed defects.

## Completion Criteria

The session is complete when the selected areas have been explored, discovered issues have been retested, results have been separated into confirmed defects and observations, and the session documentation has been prepared.
