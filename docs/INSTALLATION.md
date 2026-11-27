# Vita installation identity

The repository's sce_sys/param.sfo declares:

- **Title ID:** `RNPYDKMGN`
- **Installed application path:** `ux0:app/RNPYDKMGN`

Install the VPK through VitaShell. The path above is the application identity recorded by the package; it is not a destination for proprietary source-game files. Obtain the original game and mod separately and follow the instructions shipped with the specific port release.

The package metadata validator checks this documented path against TITLE_ID in sce_sys/param.sfo. If the package identity changes, update this document and the release notes together.
