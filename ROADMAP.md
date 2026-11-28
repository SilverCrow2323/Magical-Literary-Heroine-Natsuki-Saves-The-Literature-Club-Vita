# Roadmap — Magical Literary Heroine Natsuki Vita port

## P0 — Preserve package identity
- [x] Track SFO metadata and LiveArea assets.
- [x] Document the upstream game source and user-supplied game files.
- [ ] Reconcile the published VPK with RNPYDKMGN metadata and record its SHA-256.

## P1 — Package integrity
- [x] Add an offline SFO parser regression test with bounds checks.
- [x] Verify title ID, category, title and app version in CI.
- [x] Verify PNG signatures and parse the LiveArea XML.
- [x] Reject an accidentally committed original game/ payload.
- [ ] Pin the exact Ren'Py Vita tool/runtime revision for reproducible rebuilds.

## P2 — Physical qualification
- [ ] Record Vita model, firmware, storage layout and free space.
- [ ] Test install, first boot, game-file discovery, save/load, audio and suspend/resume.
- [ ] Record title-specific performance and rendering findings.

## P3 — Maintenance release
- [ ] Rebuild from a documented input game build.
- [ ] Compare generated metadata and asset hashes with the reviewed baseline.
- [ ] Publish notes/checksums only after physical-device qualification.

## Acceptance
CI passes; SFO remains RNPYDKMGN; no original game payload is tracked; LiveArea assets are valid; a release candidate has a separate physical Vita report. CI does not equal hardware certification.

## Release target
Maintain existing port version 1.05; no version bump or release is part of this change.
