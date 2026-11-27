# Changelog

## Unreleased

- Added a dedicated installation identity document for Title ID `RNPYDKMGN` and the installed path `ux0:app/RNPYDKMGN`.
- Extended the package metadata validator to read the dedicated installation document, so the check remains valid when practical Wiki pages are moved to the central Ren'Py Vita hub.
- Recorded the package's actual TITLE_ID from sce_sys/param.sfo; no guessed title-ID path is used.
- Corrected the title-ID path boundary expression so the validator recognizes a path ending immediately after the nine-character ID.
