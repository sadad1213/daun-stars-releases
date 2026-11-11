# Daun Stars

Official Windows builds and update metadata for Daun Stars.

[Download the latest Windows build](https://github.com/sadad1213/daun-stars-releases/releases/latest/download/DaunStars-Windows-x64.zip) · [Browse releases](https://github.com/sadad1213/daun-stars-releases/releases)

## Play

1. Download `DaunStars-Windows-x64.zip`.
2. Extract the archive into a folder you can write to.
3. Run `DaunStars.exe`.

The Windows x64 build contains the game and its resources in one executable. The current in-game interface is in Russian.

## Current prototype

- 11 playable heroes and 7 arenas.
- Solo Showdown with bots.
- Hero selection, settings, and direct-IP multiplayer.

## Release files

| File | Purpose |
| --- | --- |
| `DaunStars-Windows-x64.zip` | Ready-to-play Windows game build. |
| `update.json` | Version, download URL, archive size, and SHA-256 checksum for the updater. |
| `SHA256SUMS.txt` | SHA-256 checksums of the downloadable game archive and update manifest. |

## Update feed

Stable manifest URL:

https://github.com/sadad1213/daun-stars-releases/releases/latest/download/update.json

The manifest uses `schema_version: 1`. Game and launcher versions are tracked independently. Each component points to an archive in a specific release, so a launcher-only update can keep using the existing game build.

The launcher is not available yet: `launcher` is currently `null`. Automatic game updates and launcher self-updates will become available when the launcher is released. For now, extract the game ZIP and run the executable directly.

## Publishing updates

Publish a new release with a unique version tag. Attach the updated component archives, a complete `update.json`, and `SHA256SUMS.txt`. Mark the release as the latest full release to update the stable feed.

Keep existing tagged download URLs unchanged. An unchanged component may continue to reference its previous release archive.
