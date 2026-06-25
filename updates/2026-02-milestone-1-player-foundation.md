# Prototype Milestone 1 — Player Foundation

**Date:** February 2026  
**Phase:** Early prototype (pre-Gloomharbor architecture)

---

## What Was Proved

This milestone established the core design decisions around player movement and scene layout that carry directly into Gloomharbor.

### Input and Movement
- Dual movement modes confirmed as the right design: **FreeRoam** (smooth analog exploration) and **Combat** (precise grid-snapped movement)
- WASD + click-to-move for keyboard/mouse; gamepad support from the start
- Token rotates to face direction of movement — cardinal directions (N/S/E/W)

### Character Foundation
- D&D 5E stat block structure validated: HP, Speed (6 cells/turn default), Level, XP
- These values drive both exploration and combat — single source of truth

### Camera
- Smooth lerp follow with mouse wheel zoom
- Confirmed that a zoom range of roughly 2–7x handles both close-quarters dungeon rooms and wider outdoor areas

### Visuals
- High-resolution DungeonDraft map imported as a background image (not a tile grid)
- Token placed on top of the background — confirmed the layering approach: background → walls → tokens
- This visual model (painted background + token overlay) is the foundation Gloomharbor builds on

---

*Note: This prototype was used to validate design decisions. The Gloomharbor engine is a ground-up rebuild on a new tech stack — see the [June 2026 pivot entry](./2026-06-pivot-to-gloomharbor.md) for context.*
