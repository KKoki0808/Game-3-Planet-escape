# Planet Escape — SFX by ElevenLabs (11.ai)

**Documentation-only repository. The Unity source project and Windows executable are not distributed here while their asset distribution conditions are being confirmed.** This repository contains the development log, credits, rights review and submission documents. It is not a rebuildable Unity project or a playable download.

AME 294 — Portfolio Game 3. A third-person 3D survival game built with **Unity 6.3 LTS (6000.3.27f1)**.

Your spacecraft has crashed. Recover three repair parts from three areas, return to the ship, repair it, and escape.

| Area | Challenge | Repair part |
| --- | --- | --- |
| Rocky Canyon | Jump across graded rock platforms; use the midpoint checkpoint | Navigation Chip |
| Drone Base | Use cover and patrol gaps to avoid four drones and seven cameras | Rocket Engine |
| Alien Nest | Take the rifle and destroy all four egg nests to unlock the reward | Power Core |

## Windows download

A Windows64 build is complete locally as `PlanetEscape_Windows64.zip` (78,562,854 bytes, approximately 79 MB).
**It has not been uploaded.** Unity source and Windows build distribution are pending the conditions in [PUBLICATION_STATUS.md](PUBLICATION_STATUS.md). Only documentation is being published; no raw model, texture or audio assets are included.

[GitHub Releases — download will appear here after publication](https://github.com/KKoki0808/Game-3-Planet-escape/releases)

Once available, extract the entire ZIP and run `PlanetEscape_Build/PlanetEscape.exe`. Unity Editor is not required. Keep the EXE, data folder, DLLs, MonoBleedingEdge and D3D12 files together. Alt+F4 closes the game.

## Open the full Unity project (when access is permitted)

A documentation-only publication does **not** contain a rebuildable Unity project. The following instructions apply only to the complete local project or a future authorized full-source release.

1. Install Unity 6000.3.27f1 through Unity Hub; add Windows Build Support to rebuild the Windows player.
2. Obtain the authorized full project. If supplied through Git, use Git LFS and `git lfs pull` for its six large source GLBs.
3. Open the repository folder in Unity Hub. Let Unity restore the pinned packages and import Assets.
4. Open `Assets/PlanetEscape/Scenes/PlanetEscape.unity`, press Play, and select **BEGIN EXPEDITION** or press Enter.

The existing scene is configured. Scene-generation menus are unnecessary for normal play. The original private Unity project keeps Assets and their.meta files, Packages/manifest.json and packages-lock.json, and ProjectSettings; Library/Temp/Logs/builds are regenerated or distributed separately. The original SpaceSalvageRun and SampleScene files remain available, disabled in the submission build list.

## Controls

| Input | Action |
| --- | --- |
| WASD | Move relative to the camera |
| Shift | Run |
| Space | Jump; press again in the air for a backpack jet jump |
| Arrow keys / right mouse drag | Orbit the camera |
| E | Take the rifle at the nest entrance; repair/launch beside the ship after collecting all three parts |
| F / left mouse button | Fire while armed inside Alien Nest |
| Enter | Begin; retry on Game Over; restart after success |
| R | Reset all progress on Game Over; restart after success |

Canyon falls, detection and alien attacks cost health. A repair-part pickup restores health and counts only once. At zero health, **Retry — Keep Parts** returns to the ship with full health and retains recovered parts during the current run. **Reset All Progress** starts a fresh expedition. Closing the application ends the session; there is no disk save.

After repair, the ship levels, returns to its original clean material, plays its startup cue, then lifts off. The escape sound stops on success. The HUD shows hearts, repair progress and colored entrance trails: yellow Canyon, blue Drone Base, purple Alien Nest.

## Build and verification

The existing Windows release build succeeded with 0 errors and 0 warnings and includes PlanetEscape alone at Build Index 0. All 177 distribution files were checked against the ZIP. Headless and normal Intel Iris Xe/Direct3D11 startup checks completed initialization without exceptions. **A manual standalone playthrough, visual review, audio balance and FPS benchmark have not been completed.**

No gameplay or build binary was changed for repository preparation. One-off local source-import Python utilities and the unlicensed reference photograph stay on the author's machine and are not required to open or rebuild the checked-in native Unity scene.

## Development and asset records

- [Chronological prompt and development record](PROMPT_LOG.md)
- [Detailed implementation log](Assets/PlanetEscape/DEVELOPMENT_LOG.md)
- [Asset credits and unresolved permissions](ASSET_CREDITS.md)
- [Per-use rights review and submission options (Japanese)](ASSET_RIGHTS_REVIEW.md)
- [Machine-readable asset inventory](ASSET_LICENSE_INVENTORY.csv)
- [Unity package notices](THIRD_PARTY_NOTICES.md)
- [Publication status and remaining actions](PUBLICATION_STATUS.md)

This is not a blanket open-source license for the models, textures or audio. Asset-specific rights must be confirmed before redistribution.

## Asset attribution and publication scope

Sound effects were generated by the project author using **ElevenLabs (11.ai)** on the Free plan. This is a **noncommercial university assignment**. Models were generated by the author using Tripo on its Free plan. The sky was generated with the OpenAI image tool; the reference photograph is separate and is not distributed. Provider credits do not grant recipients a blanket license to extract or redistribute the media.

The intended public Release title is **Planet Escape — SFX by ElevenLabs (11.ai) — Windows64**. The title and this README supply an explicit attribution proposal; whether external title placement alone suffices for the unchanged game binary remains to be confirmed. No raw MP3 download is offered. This documentation does not claim that a public game Release already exists.

- [Shortest submission route and publication file decisions](SUBMISSION_PUBLICATION_PLAN.md)
- [Unsent provider inquiry drafts](LICENSE_INQUIRIES.md)
- [Conditional Windows Release draft](RELEASE_DRAFT.md)
- [File-level held media and derivatives](PUBLICATION_FILE_DECISIONS.csv)

## This public repository

Only text documentation and retained third-party license notices are included. The original Unity project and its existing Git history are preserved separately. This repository starts from an independent documentation-only history and includes no historical model or audio blobs. See PUBLICATION_ALLOWLIST.csv for the published file list and checksums. Draft inquiries and Release text are labelled as drafts; no provider reply or game Release is claimed.
