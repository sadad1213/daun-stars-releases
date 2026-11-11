# Daun Stars

Official Windows builds and update metadata for Daun Stars.

[Download the launcher](https://github.com/sadad1213/daun-stars-releases/releases/latest/download/DaunStars.exe) · [Browse releases](https://github.com/sadad1213/daun-stars-releases/releases)

## Play

Download **DaunStars.exe**, save it in a writable folder, and run it. The launcher opens fullscreen, fades into the loading screen, checks for updates, and installs the game automatically. At 99% it starts the fullscreen game and hands over to its matching loading screen.

The launcher requires .NET Framework 4.8 or newer, included in current Windows 10/11 releases. The current game and launcher interface is in Russian.

To install the game manually, download [DaunStars-Windows-x64.zip](https://github.com/sadad1213/daun-stars-releases/releases/latest/download/DaunStars-Windows-x64.zip), extract it, and run `DaunStars.exe`.

## Game

- 11 playable heroes and 7 arenas.
- Solo Showdown with bots.
- Hero selection, settings, and direct-IP multiplayer.

## Release files

| File | Purpose |
| --- | --- |
| `DaunStars.exe` | Standalone launcher with embedded artwork and font. |
| `DaunStarsLauncher-Windows-x64.zip` | Launcher self-update package. |
| `DaunStars-Windows-x64.zip` | Ready-to-play Windows x64 game build. |
| `update.json` | Independent game/launcher versions, download URLs, sizes, and SHA-256 checksums. |
| `SHA256SUMS.txt` | Checksums for the release downloads. |

## Updates

Stable feed: [update.json](https://github.com/sadad1213/daun-stars-releases/releases/latest/download/update.json).

The manifest uses `schema_version: 1`. Game and launcher versions are tracked independently, and each component points to its archive in a specific release. An unchanged component can continue to reference its previous archive.

Game files and launcher logs are stored under `%LOCALAPPDATA%\DaunStars`. Updates use a new version directory and preserve the previous game. If the feed is unavailable, a valid installed game can start offline. Self-updates use a temporary worker and retain a backup of the launcher executable.

No GitHub account is needed to play.
