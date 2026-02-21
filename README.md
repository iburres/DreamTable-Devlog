# DreamTable — Development Log

> A top-down 2D tactical RPG built in Unity 6, inspired by virtual tabletop platforms like FoundryVTT and Roll20. Play solo or with friends across richly detailed maps with D&D 5E-style combat rules.

---

## What is DreamTable?

DreamTable aims to bring the feel of a digital tabletop session to a standalone game — custom maps, animated character tokens, turn-based grid combat, and free-roam exploration. Think of it as the game *inside* your TTRPG session.

**Engine:** Unity 6 (URP)
**Genre:** Top-down tactical RPG
**Status:** Early development

---

## Progress

### ✅ Milestone 1 — Player Foundation *(Feb 2026)*
- New Input System action maps (WASD, mouse click, gamepad)
- Grid-based movement controller with **FreeRoam** and **Combat** modes
  - FreeRoam: smooth analog movement for exploration
  - Combat: grid-snapped turn-based movement
- D&D 5E-style stat block (HP, Speed, Level, XP)
- Smooth camera follow with **mouse wheel zoom**
- Cardinal direction token rotation (token faces direction of movement)

### ✅ Milestone 2 — Scene & Visuals *(Feb 2026)*
- DungeonDraft map loaded as scene background (40×40 cells, 150px/cell)
- Custom token on player
- Dragon token staged for enemy use
- Sorting layer stack: map → walls → tokens

### ✅ Milestone 3 — Combat Mode Core *(Feb 2026)*
- **C key** toggles combat mode on/off
- Grid overlay appears in combat (40×40 cells, LineRenderer-based, URP-safe)
- Movement budget: 6 cells/turn drawn from `PlayerStats.Speed`
- Budget guard on `MoveToCell` — token stops when cells are exhausted
- **End Turn** resets budget (keyboard: Enter, gamepad: left shoulder)
- Combat HUD: live "Movement: X / 6" label + End Turn button

### 🔲 Up Next
- Initiative tracker and turn order
- Enemy placement and basic AI
- Scene transitions / multiple maps
- Fog of war / vision radius
- Inventory and item system
- UI: HUD, health bars, turn order panel

---

## Tech Stack

| Layer | Tool |
|---|---|
| Engine | Unity 6000.3.9f1 |
| Render pipeline | URP (Universal Render Pipeline) |
| Input | Unity Input System 1.11.2 |
| Maps | DungeonDraft |
| Tokens | Custom tokens |
| Version control | Git / GitHub |

---

## Contributing

The source code and assets are in a private repository. If you're interested in contributing — art, code, maps, sound, or playtesting — open an **Issue** or **Discussion** here to get in touch.

---

## Screenshots

*Coming soon — first playable build in progress.*

---

## Follow Along

Updates are posted here as milestones are reached. Watch/star the repo to get notified.
