# Pivot — Gloomharbor: New Direction, New Foundation

**Date:** June 2026

---

## What Changed and Why

After completing early combat and movement prototypes that validated the core design decisions, we made a deliberate decision to pivot the entire project — engine, tech stack, and scope.

The original prototype proved the concept: turn-based combat, token movement, and a grid overlay all worked as intended. The design decisions it validated — dual movement modes, event-driven combat, painted background maps with token overlays — carry forward unchanged into Gloomharbor.

The new direction is built on web technologies running inside a native desktop shell — the same foundational approach that powers the best virtual tabletop platforms available today. This gives us a rendering pipeline that handles high-resolution painted maps and animated tokens beautifully, a real-time multiplayer layer that works peer-to-peer without a dedicated game server, and a UI system that lets the editor panels feel polished without a separate UI engine.

---

## The Product Is Now Bigger

What started as "a top-down RPG" is now a full platform:

**Gloomharbor** is both a game and a creation suite. The editor ships with the game. Players can build and share their own RPG games and adventure modules — campaigns a Game Master can run for a group in virtual tabletop mode. No external tools required.

The game world itself — a hidden dark fantasy continent shrouded in ancient fog, unknown to the outside world — became the name and the identity of the entire platform.

---

## Architecture Completed

A full architectural design session produced decisions on every major system:

- One-app mode switching: game, editor, and virtual tabletop host all in the same binary
- Hybrid map system: geometry layer (walls, doors, sight lines) always separate from the visual layer (painted backgrounds or imported maps)
- Turn-based combat running the D&D 5th Edition SRD ruleset
- Node graph dialogue editor with a Baldur's Gate-style runtime panel
- Built-in Lua scripting for encounter automation
- Atmospheric lighting for the demo; full line-of-sight and fog of war for multiplayer
- Full party control: player, companions, and NPCs are all distinct characters with their own stats, motivations, and dialogue trees
- Layered token appearance system: armor type, cloak, color tinting — customizable per character

---

## Infrastructure Set Up

- Private development repository created and pushed
- Docker development container configured — Vite renderer runs in container, Electron connects natively
- CI pipeline active — every pull request triggers an automated build verification
- Branch-per-feature workflow enforced: no direct commits to main

---

## Kickstarter Demo Target

The first playable milestone is a short haunted mansion demo showcasing:
- Turn-based combat with a fighter and two companions
- Scripted traps and environmental triggers
- Branching NPC dialogue
- Atmospheric lighting (torches, darkness)
- A puzzle or two
- A UI walkthrough of the editor and planned post-funding features

This demo will anchor the Kickstarter campaign, which aims to fund a team of artists to produce the high-quality painterly assets the game's vision requires.

---

## What Carries Forward from the Unity Prototype

The core design decisions survived the pivot intact: turn-based grid combat, top-down token movement, D&D 5E-style stat blocks, and the vision of a VTT-quality presentation in a standalone game. Two months of design work translated directly — only the implementation layer changed.

---

*Next update: Kickstarter demo — first playable build.*
