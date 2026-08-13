# Knowledge modules 2026.03.05 r1

This release contains the 13 optional offline knowledge modules referenced by the Genesis Android application.

- Binary release assets: 15
- Complete installed payload: 6,322,401,280 bytes
- Binary download payload: 4,113,463,323 bytes
- Four smaller modules are distributed as complete SQLite assets.
- Eight larger modules use one deterministic gzip asset each.
- The largest module uses one deterministic gzip byte stream divided into three ordered Release assets. The app treats the parts as a continuous gzip stream and does not retain a second complete compressed copy on the phone.
- The app validates every part, the complete compressed stream, and the decompressed SQLite size, SHA-256, pack ID, version, entry count, storage format, and index version.
- See `SHA256SUMS.txt`, `knowledge_pack_manifest.json`, and `THIRD_PARTY_NOTICES.md` in the repository.

These assets are optional. The APK's small core worldbuilding knowledge pack remains available without downloading this release. Ordinary users do not need to handle ZIM files, SQLite paths, URLs, or checksums.
