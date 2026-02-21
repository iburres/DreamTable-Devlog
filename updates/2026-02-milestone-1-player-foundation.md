# Milestone 1 — Player Foundation

**Date:** February 2026

## What was built

This milestone established the core player character and scene infrastructure.

### Input System
- Created `DreamTableInputActions.inputactions` with full **Player** and **UI** action maps
- Bindings for Keyboard & Mouse and Gamepad control schemes
- Actions: Move (WASD + arrows + left stick), PointAndClick, Interact, Attack, OpenInventory, Cancel

### Player Controller
- Dual movement modes:
  - **FreeRoam** — smooth analog WASD movement and click-to-move over exploration maps
  - **Combat** — grid-snapped cardinal movement (called by CombatManager, coming soon)
- Token rotates to face direction of movement (cardinal: N/S/E/W)
- `PlayerStats` component: MaxHP, CurrentHP, Speed (D&D 5E default 6 cells/turn), Level, XP

### Camera
- Smooth lerp follow with configurable speed
- **Mouse wheel zoom** — range 2–7 orthographic units, starts at 3.5

### Visuals
- DungeonDraft map imported as background (6000×6000px, 40×40 cells)
- Custom token wired to player prefab
- Dragon token staged for future enemy use
- Sorting order stack: Background (−10) → Walls (0) → Tokens (1)
