# Releases

Notarized builds of my Mac apps. Each app reads its own tags (`<app>-vX.Y.Z`) through [AppUpdater](https://github.com/erikrole/AppUpdater). Source code lives elsewhere.

## Stable feeds

Each file in `feeds/` lists verified stable releases for one macOS app. AppUpdater selects a compatible version and verifies the archive's SHA-256 before extraction.

To refresh a feed, verify the signed candidate and its public download, then run AppUpdater's `scripts/update-stable-feed.py` with the GitHub release metadata and tested archive. Publish a new version when an archive changes.
