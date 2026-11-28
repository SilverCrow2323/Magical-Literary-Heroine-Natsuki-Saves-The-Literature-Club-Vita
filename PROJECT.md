# Project: Magical Literary Heroine Natsuki — PlayStation Vita port

## Purpose
Maintain the Vita-side application metadata and LiveArea package shell for the Ren'Py conversion of Magical Literary Heroine Natsuki. This is a port/package repository, not the source repository for the original game.

## Users and use cases
Vita owners install the VPK and supply their own legally obtained original game files. Maintainers verify title identity, LiveArea assets, compatibility notes and release packaging. Testers record boot, save/load, rendering, audio and performance on real hardware.

## Scope and boundaries
In scope: Vita SFO metadata, icon/background/startup assets, installation instructions, compatibility notes and reproducibility evidence. Out of scope: redistribution of the original game's game/ payload, DRM/license bypass, claims of upstream ownership, or changes to the Ren'Py Vita runtime.

Original game source: https://www.mlhnstlc.com
Conversion tool: https://github.com/SonicMastr/renpy-vita

## Target and dependencies
- PlayStation Vita / PlayStation TV with a compatible homebrew environment.
- Ren'Py Vita runtime, VitaShell and user-supplied original game files.
- Rebuilds must record exact tool/runtime revisions, input game build identifier and generated VPK hash.

## Package architecture
- sce_sys/param.sfo: expected TITLE_ID RNPYDKMGN, title Magical Literary Heroine Natsuki, app version 1.05.
- sce_sys/icon0.png, pic0.png and livearea/contents/: application presentation.
- README.md and wiki-source/: installation, source attribution and troubleshooting.
- The user supplies the original game's game/ directory at the documented path.

## Safety and quality
Never commit proprietary game payloads or user saves. SFO parsing must check offsets and lengths. Installation instructions must distinguish known bugs from untested behavior. CI metadata checks are not a physical Vita certification.

## Verified baseline
The tracked SFO reports RNPYDKMGN / Magical Literary Heroine Natsuki / 1.05; the repository contains package metadata and LiveArea assets, not the original game payload. Physical runtime qualification remains a separate release gate.
