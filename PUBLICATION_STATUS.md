# Publication status — Web game, trailer and documentation

Status date: 2026-10-27.

**Play:** https://kkoki0808.github.io/Game-3-Planet-escape/

**Trailer:** https://kkoki0808.github.io/Game-3-Planet-escape/trailer/

Repository: https://github.com/KKoki0808/Game-3-Planet-escape

## Authorized scope

The author explicitly approved **Web publication only**, superseding the earlier no-uncleared-media publication restriction for this compiled Web build. The author did not claim that provider permission questions had been resolved. Asset rights reviews therefore remain conditional and are not changed to “cleared.”

- `main`: documentation, prompt/development logs, credits, rights inventories and legal notices.
- `gh-pages`: compiled Web game and generated page resources, plus the separately supplied trailer, poster, video player and music credit, served by GitHub Pages.
- Not published: full Unity source, original GLB/FBX/MP3 assets, reference images, Windows EXE/ZIP.

The Web player embeds game meshes, textures, audio and compiled code as a playable production. It is not an asset pack, and embedded media is not claimed to be impossible to extract. The reference photograph remains absent from runtime use. Original local Unity files/history and Windows build are preserved separately; no force push or history rewrite is used.

## Build and verification

Unity 6000.3.27f1 Web build: succeeded, zero errors and zero warnings, PlanetEscape scene only. Web compression uses Gzip with decompression fallback; the Web player uses no WebAssembly threads. The page includes the ElevenLabs (11.ai) title credit and responsive sizing. See WEB_BUILD_MANIFEST.csv for deployed file hashes.

Browser checks on this PC confirmed loading, the start screen, beginning play, forward movement, arrow-key camera orbit and double jump with visible jet exhaust; no browser warning/error was captured in that local check. A complete mission playthrough, browser shooting/egg unlock/reward completion, audio listening/balance, FPS benchmark and other devices remain unverified. The public HTTPS URL was also opened and those same initial controls were checked again. All 17 public runtime files matched deployment SHA256 values. No public-browser error/warning was captured in that check. The latest prompt-log entry records the actual publication result.

## Remaining items

| Item | Status |
| --- | --- |
| Browser play | Web build authorized for publication; link above |
| Full Unity source | Not distributed; original/derived model redistribution and raw audio restrictions remain |
| Windows download | Not uploaded; not included in the Web-only approval |
| Provider licenses / sky reference-input rights | Recorded questions remain unresolved; author publication approval is separate from rights clearance |
| Provider replies | Inquiry drafts only; none invented |
| Full manual playthrough | Still to be completed |

Prior preparation documents and chronological entries describe the state when written. This status file and the latest prompt-log entry describe the current publication scope. Free-plan self-generation and noncommercial university purpose remain user-confirmed facts.


## Supplied trailer publication

The user explicitly requested publishing the provided cinematic MP4 and featuring it near the top of README. The MP4 is preserved byte-for-byte; its 45-second H.264/AAC format was decoded successfully. Six sampled frames were checked visually. Creation/revision prompts were retrieved from the trailer-editing conversation and translated into English in PROMPT_LOG. Music credit for Kevin MacLeod’s “The Descent” (CC BY 4.0) is included on the player page, README/credits and in the existing final title card. No raw soundtrack MP3 is uploaded. TRAILER_MANIFEST.csv records these four added page/media files separately; the original Web player hashes in WEB_BUILD_MANIFEST.csv remain unchanged. This additional publication request does not authorize Windows or full-source release and does not resolve outstanding game-asset rights questions.
