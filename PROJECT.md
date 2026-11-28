# Project definition — Magical Literary Heroine Natsuki Saves the Literature Club! Vita

## Product and boundary
A PS Vita Ren'Py adaptation package for the **Magical Literary Heroine Natsuki Saves the Literature Club!** DDLC mod. This repository is a Vita package/installation layer, not the original DDLC game or the mod's upstream source.

## Upstream and runtime
- Base game: [Doki Doki Literature Club on Steam](https://store.steampowered.com/app/698780/Doki_Doki_Literature_Club/).
- Mod: [MLHNSTLC project site](https://www.mlhnstlc.com/).
- Vita runtime/port lineage: [Ren'Py Vita](https://github.com/SonicMastr/renpy-vita) and [SonicMastr's DDLC Vita port](https://github.com/SonicMastr/Doki-Doki-Literature-Club-Vita).
- Base-game and mod content must be sourced under their own terms; do not bundle files without permission.

## Users and target
PS Vita users installing the modded port. Exact app ID, install path, firmware baseline and runtime revision still require verification from the package metadata and a device.

## Architecture and dependencies
The tracked package shell contains SFO/LiveArea metadata and artwork plus source/install documentation. It depends on the base game, mod payload and Ren'Py Vita runtime.

## Security and quality
Keep base-game, mod and port attribution distinct. Validate package metadata and local LiveArea paths. Do not infer the install path from the repository name.

## Verified baseline
The README identifies the base game, mod and Vita port dependencies. The repository does not establish a hardware-tested release in its README; automated metadata checks are not gameplay certification.

## Release acceptance
Confirm app identity and installation path from SFO, document exact required payload and source versions, pass package integrity CI, and record a real Vita test of boot, script progression, save/load and mod-specific behaviour.