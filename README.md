# Gloomharbor — Development Log

> Built by **DreamTable Studios**

---

## What is Gloomharbor?

Gloomharbor is a top-down 2D dark fantasy RPG and a self-contained RPG creation platform — both in one application. Play the game, then open the built-in editor and build your own.

The world of Gloomharbor is a hidden continent locked inside the Bermuda Triangle, invisible to the outside world. Ships and planes that vanish there didn't disappear — they arrived.

---

## Two Products, One App

### The Game
A dark fantasy RPG set in the world of Gloomharbor. Turn-based combat, party-based exploration, atmospheric lighting, branching dialogue, and scripted encounters — built on the D&D 5th Edition System Reference Document (SRD).

### The Editor
A full suite of creation tools bundled with the game — no external software required:
- **Map Editor** — build indoor and exterior areas from scratch, or import from tools like DungeonDraft
- **Token Editor** — create and customize player, NPC, and monster tokens with layered appearance
- **Dialogue Editor** — build branching conversations with a visual node graph
- **Script Editor** — write encounter logic and automation in a built-in scripting environment
- **Character Editor** — design full character sheets with stats, abilities, and token appearance
- **Module Packaging** — export a complete game or adventure module as a single shareable file

Developers can build and distribute their own standalone RPG games or playable adventure modules — campaigns a Game Master can run for a group of players in virtual tabletop mode.

---

## Vision

The goal is to give developers and storytellers — including those with limited coding experience — everything they need to create and share a real, playable RPG game without purchasing additional tools. Think Neverwinter Nights, but as a modern top-down platform with high-quality painterly art, animated environments, and full virtual tabletop support.

Gloomharbor is planned for release on Steam, with the editor included as a first-class selling point.

---

## Tech Foundation

Built on a modern, battle-tested web technology stack running inside a native desktop shell:
- **Rendering:** PixiJS v8 with WebGL 2.0
- **Real-time multiplayer:** WebSocket + WebRTC peer-to-peer
- **Scripting:** Lua sandbox
- **Data:** LevelDB

Evolved from an earlier prototype — the engine foundation carries forward, now significantly expanded.

---

## Ruleset Support

- **Demo / Early Access:** D&D 5th Edition SRD (Creative Commons, fully open)
- **Full Release:** Pathfinder 2nd Edition (open license from Paizo)
- Ruleset engine is data-driven — additional systems can be added as content packs

---

## Roadmap

| Milestone | Description | Status |
|-----------|-------------|--------|
| Foundation | Architecture design, dev infrastructure, engine foundation | ✅ Complete |
| Kickstarter Demo | Short playable haunted mansion — combat, dialogue, traps, exploration | 🔄 In Progress |
| Kickstarter Campaign | Fund artist team for high-quality game assets | ⏳ Planned |
| Full Game — Alpha | Complete Gloomharbor world, all editor tools functional | ⏳ Planned |
| Steam Release | Game + bundled editor shipped on Steam | ⏳ Planned |

---

## Development Updates

See the [`updates/`](./updates/) directory for detailed milestone entries.

| Date | Entry |
|------|-------|
| June 2026 | [Pivot — Gloomharbor: New Direction, New Foundation](./updates/2026-06-pivot-to-gloomharbor.md) |
| Feb 2026 | [Milestone 3 — Combat Mode Core](./updates/2026-02-milestone-3-combat-mode-core.md) |
| Feb 2026 | [Milestone 1 — Player Foundation](./updates/2026-02-milestone-1-player-foundation.md) |

---

## Follow Along

Updates are posted here as milestones are reached. Watch or star the repo to get notified.

---

*DreamTable Studios — building worlds worth exploring.*
