# apple-platform-skills

Claude Code skills for Apple platform development — visionOS, SpriteKit, and GameKit multiplayer.

Install all skills:
```bash
npx skills add ibrews/apple-platform-skills
```

Or install individually by referencing the skill name after setup.

## Skills

### `visionos-shareplay`
SharePlay and GroupActivities development for visionOS and iOS. Covers GroupSession lifecycle, GroupSessionMessenger state sync, spatial personas, ImmersiveSpace integration, and common pitfalls (the `session.join()` trap, session retention, simulator limitations).

### `spritekit-ios`
SpriteKit 2D game development. Covers the Y-up coordinate system, physics bitmasks (and the UInt32 overflow trap), SKAction sequences/groups, texture atlases for animation, SKTileMapNode, game loop method responsibilities, and performance targets.

### `gamekit-multiplayer`
GameKit real-time and turn-based multiplayer. Covers GKLocalPlayer auth (must happen before everything), GKMatch vs GKMatchmakerViewController, reliable vs unreliable data transport, player connect/disconnect handling, sandbox vs production Game Center, and common silent-failure traps.

## Things to Try

1. **Install and test visionOS SharePlay skill** — open a SharePlay project in Claude Code and ask it to add a new synchronized game state message; the skill will guide correct session lifecycle and messenger usage.
2. **Debug a physics collision** — describe a contact detection problem in a SpriteKit project; the skill surfaces the bitmask ordering trap and the UInt32 overflow limit immediately.
3. **Set up GameKit matchmaking from scratch** — ask Claude to add multiplayer to an existing iOS game; the skill ensures auth is wired before matchmaking and `expectedPlayerCount` gates game start correctly.
4. **Add SharePlay to a visionOS ImmersiveSpace** — the skill covers the exact `.task` pattern for opening a shared immersive space when a session activates.
5. **Optimize a SpriteKit scene that's dropping frames** — the skill gives concrete node count targets, explains SKShapeNode vs SKSpriteNode cost, and shows which debug overlays to enable.

## About

Built by [Agile Lens](https://agilelens.com) — XR studio and Apple platform developers since 2009. These skills reflect real patterns from shipping visionOS and iOS apps including SharePlay multiplayer experiences.
