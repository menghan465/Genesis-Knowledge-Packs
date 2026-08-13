# Knowledge modules 2026.03.05 r1

This release contains the 13 optional offline knowledge modules referenced by the Genesis Android application.

- Binary release assets: 13
- Complete installed payload: 6,322,401,280 bytes
- Binary download payload: 4,113,463,323 bytes
- Four smaller modules are distributed as complete SQLite assets.
- Nine larger modules use deterministic gzip transport. The app downloads and decompresses them as a stream, without retaining a second full compressed copy on the phone.
- The app validates the compressed asset size and SHA-256, then validates the decompressed SQLite size, SHA-256, pack ID, version, entry count, storage format, and index version.
- See `SHA256SUMS.txt`, `knowledge_pack_manifest.json`, and `THIRD_PARTY_NOTICES.md` in the repository.

These assets are optional. The APK's small core worldbuilding knowledge pack remains available without downloading this release. Ordinary users do not need to handle ZIM files, SQLite paths, URLs, or checksums.
