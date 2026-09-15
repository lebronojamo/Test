# Crownfall Arena — HTML update feed

This folder supplies verified updates to the downloadable Crownfall Arena HTML game. Players keep opening their existing HTML; the game runs in that document and preserves its browser save location.

The HTML checks `latest.json` in the background, verifies the numbered package with SHA-256, and caches it separately from game progress. Updates take effect on the next opening. The embedded game remains the offline fallback.

Current release: **2026.09.15.1**, sequence **1**.

## Publishing

Publish a new immutable `release-N.json` first, then update `latest.json` last. Always increase the sequence. Keep the original asset baseline and compatible loader/save protocol 1. The baseline and release builder are included in the project's Crownfall Arena QA/source archive and Updates Guide.

Do not replace a numbered release with different bytes or publish backwards. No player saves, credentials or contacts belong in this folder. SHA-256 checks integrity; publisher trust depends on this repository and HTTPS.

This game is unofficial and is not endorsed by Supercell. Artwork attribution and the Supercell Fan Content Policy notice are included in the game.
