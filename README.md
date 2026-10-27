# PLANET ESCAPE — SFX by ElevenLabs (11.ai)
### A 3D Sci-Fi Survival Adventure | AME 294 — Portfolio Game 3

**Developed with Unity 6.3 LTS, OpenAI Codex, Tripo, and ElevenLabs**

> **Current public scope: documentation only.** The Unity source project and Windows build are not publicly distributed while their asset distribution conditions are being confirmed. This repository is not a playable download or a complete, rebuildable Unity project.

[Development & AI Prompt Log](PROMPT_LOG.md) · [Asset Credits](ASSET_CREDITS.md) · [Publication Status](PUBLICATION_STATUS.md)

## About the Game

*Your spaceship has crashed on an unknown planet. Explore, survive, repair, and escape.*

**Planet Escape** is a third-person 3D adventure game combining platforming, stealth, and combat in a small, interconnected world.

Players explore three distinct areas to recover three missing spaceship components. Each area introduces a different challenge, requiring different strategies and skills.

Once all three repair parts have been collected, the player must return to the crashed spaceship, repair it, and escape the planet.

**Objective:** Collect all 3 repair parts, survive the planet's dangers, and launch your spaceship.

## Explore Three Unique Areas

### 1. Rocky Canyon — Platforming Challenge

Navigate a rocky canyon filled with elevated platforms, narrow landing areas, and dangerous gaps.

- Jump across rocks using normal and double jumps.
- Overcome increasingly challenging platforming sections.
- Use the checkpoint to recover from failed jumps.
- Collect the **Navigation Chip**.

**Core skill:** Movement and precision.

### 2. Drone Base — Stealth Challenge

Infiltrate a futuristic security base guarded by four patrol drones and seven surveillance cameras.

- Observe enemy patrol patterns.
- Hide behind cargo containers, trucks, and defensive walls.
- Avoid the visible surveillance fields; detection causes health loss.
- Reach the secured area and recover the **Rocket Engine**.

**Core skill:** Observation and strategy.

### 3. Alien Nest — Combat Challenge

Explore an underground alien nest infested with hostile spider-like creatures.

- Find and equip a futuristic rifle.
- Fight aggressive alien spiders.
- Destroy four egg nests to unlock the final repair component.
- Recover the **Power Core**.

**Core skill:** Aiming, combat, and survival.

## Gameplay Features

- Third-person exploration with freely controlled camera movement
- Running, jumping, and jet-assisted double jumping
- Three distinct gameplay styles: platforming, stealth, and shooting
- Health and damage mechanics
- Repair-part collection and progress tracking
- Checkpoints and retry options
- Sound effects created with ElevenLabs
- A spaceship repair and takeoff sequence
- Win and Game Over screens with restart functionality

### Reward, Damage, End

The game combines rewards, damage, and a clear ending:

| Element | Implementation |
|---|---|
| **Reward** | Collect three repair parts and restore health |
| **Damage** | Canyon falls, drone/camera detection, and contact with alien enemies |
| **End** | Repair the spacecraft and escape to win, or lose all health to reach Game Over |

Players can retry after failure or restart the expedition.

## Controls

| Key | Action |
|---|---|
| W / A / S / D | Move |
| Shift | Run |
| Space | Jump / Double Jump |
| Arrow keys or Right Mouse Drag | Rotate camera |
| E | Pick up rifle / Repair and launch spaceship after collecting all three parts |
| F or Left Mouse Button | Shoot in Alien Nest |
| Enter | Begin / Retry / Restart |
| R | Reset progress from Game Over / Restart after success |
| Alt + F4 | Exit the Windows game |

Movement is relative to the camera direction. Keyboard-based camera controls are supported. Press Space once to jump, release it, then press again for the backpack jet jump.

Each repair part can be collected only once, and picking one up restores health. At Game Over, **Retry — Keep Parts** returns the player to the ship with recovered parts retained for the current run. **Reset All Progress** starts a fresh expedition. Progress is not saved after closing the application.

## Built with Artificial Intelligence

Planet Escape was developed using AI throughout the game development process.

**OpenAI Codex — Programming and Unity Development**

Codex assisted with C# programming, level construction, gameplay mechanics, debugging, camera controls, enemy behavior, UI, and build preparation.

**Tripo — 3D Asset Creation**

Tripo was used to generate 3D content for the game, including environmental objects and game assets. Generated content was imported into Unity.

**ElevenLabs — Sound Design**

ElevenLabs was used to produce sound effects for spaceship systems, item collection, jet-assisted jumping, enemy behavior, and combat.

**OpenAI Image Generation — Visual References**

OpenAI image generation was used for the Milky Way sky and selected visual references, including the egg reference reported by the author. Supplied reference images are not included in this documentation repository. The prompt log distinguishes recorded prompts, retrospective summaries, translations, and reconstructed text.

### Human First → AI in the Middle → Human Last

**Human First:** I developed the concept, selected the three gameplay styles, designed the challenges, and determined how the player would progress.

**AI in the Middle:** AI tools helped generate code, 3D content, sound effects, and implementation solutions.

**Human Last:** I evaluated the results, identified gameplay and visual problems, requested improvements, and made the final creative decisions.

The development process included multiple iterations, such as balancing Rocky Canyon's difficulty, restructuring Alien Nest as an underground area, and improving third-person aiming.

For a detailed chronological record, see [PROMPT_LOG.md](PROMPT_LOG.md).

## Windows Build and How to Play

**Build status:** The Windows 64-bit version has been built successfully, with zero build errors and zero warnings.

**Distribution status:** The executable is currently not publicly available while the asset distribution conditions are being reviewed.

When an authorized release becomes available:

1. Download the Windows ZIP from [GitHub Releases](https://github.com/KKoki0808/Game-3-Planet-escape/releases).
2. Extract the entire ZIP file.
3. Keep all extracted supporting files together and run `PlanetEscape_Build/PlanetEscape.exe`.
4. Start the game and explore the planet.

Unity Editor is not required to play the Windows build.

The existing build passed automated build and startup checks. A complete manual standalone playthrough, audio balance review, and performance benchmark have not been documented. No new game test is claimed by this README update.

## Unity Project

- **Engine:** Unity 6.3 LTS (6000.3.27f1)
- **Rendering:** Universal Render Pipeline (URP)
- **Language:** C#
- **Platform:** Windows 64-bit
- **Project type:** Third-person 3D adventure

The complete Unity source project is currently not distributed in this public repository because asset redistribution permissions remain under review.

If an authorized source release becomes available, the project can be opened using the corresponding Unity Editor version. Git LFS is required to retrieve large 3D source assets.

## Development Documentation

- [Master AI Prompt Log](PROMPT_LOG.md)
- [Detailed Development Log](Assets/PlanetEscape/DEVELOPMENT_LOG.md)
- [Asset Credits](ASSET_CREDITS.md)
- [Asset Rights Review](ASSET_RIGHTS_REVIEW.md)
- [Asset License Inventory](ASSET_LICENSE_INVENTORY.csv)
- [Publication Status](PUBLICATION_STATUS.md)
- [File-by-File Publication Decisions](PUBLICATION_FILE_DECISIONS.csv)
- [Submission Plan](SUBMISSION_PUBLICATION_PLAN.md)
- [Provider Inquiry Drafts — Not Sent](LICENSE_INQUIRIES.md)
- [Third-Party Notices](THIRD_PARTY_NOTICES.md)

These records document the production workflow, AI tools, asset origins, technical decisions, and unresolved distribution questions.

## Credits and Attribution

**Game concept, creative direction, and development supervision:** Project author

**Programming assistance:** OpenAI Codex

**3D generation:** Tripo — generated by the project author using the Free plan

**Sound effects:** ElevenLabs (11.ai) — generated by the project author using the Free plan

**Sky and visual reference generation:** OpenAI image-generation tools

This project was created for a noncommercial university assignment. The intended Windows Release title is **Planet Escape — SFX by ElevenLabs (11.ai) — Windows64**. This README includes an explicit sound-effects credit; whether external title placement alone satisfies attribution for the unchanged game binary remains part of the distribution review.

Third-party and AI-generated asset distribution rights are addressed individually in the asset documentation. Public documentation does not grant permission to redistribute the underlying models, textures, or audio.

## Current Publication Status

This GitHub repository currently contains **documentation only**.

The Unity source project and Windows executable have not been publicly distributed because their asset distribution conditions are still being reviewed.

The local Windows build is complete, but the public Release is not yet available. This repository is not currently a playable download or a complete, rebuildable Unity project.

The original Unity project, existing Git history, and local Windows build are preserved separately. This public repository uses an independent documentation-only history; model, image, audio, and build files are not hidden in its earlier commits. [PUBLICATION_ALLOWLIST.csv](PUBLICATION_ALLOWLIST.csv) lists the published documents and their checksums.

See [Publication Status](PUBLICATION_STATUS.md) for details.

---

**Arizona State University | AME 294: Games and AI | Portfolio Game 3**

*Explore. Survive. Repair. Escape.*