# Prototype Milestone 3 — Combat Mode Core

**Date:** February 2026  
**Phase:** Early prototype (pre-Gloomharbor architecture)

---

## What Was Proved

This milestone delivered the first functional combat pass and validated the core turn-based design decisions that Gloomharbor carries forward.

### Combat Flow
- Combat starts when the player enters a trigger zone or initiates an attack — not from a key press
- Turn-based with a movement budget: each character gets a set number of cells per turn (6 by default, per D&D 5E Speed)
- Movement is blocked when the budget is exhausted — confirmed this feels correct as a player experience
- **End Turn** resets the budget and passes control — keyboard and gamepad both supported

### Grid Overlay
- A grid overlay appears when combat starts and hides when it ends
- Visual parameters confirmed: subtle white lines at low opacity sit above the map but below tokens
- Cell size and grid dimensions tie directly to the map scale

### Combat HUD
- Live movement label ("Movement: 4 / 6") updates in real time as the player moves
- End Turn button visible during combat, hidden during exploration
- These two elements proved sufficient for a readable turn-based UI without clutter

### Event Architecture
- Combat state broadcasts events that other systems (grid, HUD, AI) listen to without tight coupling
- This event-driven pattern is central to Gloomharbor's architecture — systems communicate through an event bus, not direct references

### Asset Research
- WebP confirmed as preferred format for high-resolution tokens — best balance of quality and file size
- PNG and WebP both supported in the token loading pipeline

---

*Note: This prototype was used to validate design decisions. The Gloomharbor engine is a ground-up rebuild on a new tech stack — see the [June 2026 pivot entry](./2026-06-pivot-to-gloomharbor.md) for context.*
