# Knowledge modules 2026.03.05 r1

This release contains the 13 optional offline knowledge modules referenced by the Genesis Android application.

- Binary release assets: 14
- Complete installed payload: 6,322,401,280 bytes
- The `gutenberg-en-lcc-b` database is split into `.part01` and `.part02`; the app downloads and concatenates them in order, checks each part, then verifies the complete database.
- All other databases are single assets.
- See `SHA256SUMS.txt`, `knowledge_pack_manifest.json`, and `THIRD_PARTY_NOTICES.md` in the repository.

These assets are optional. The APK's small core worldbuilding knowledge pack remains available without downloading this release.
