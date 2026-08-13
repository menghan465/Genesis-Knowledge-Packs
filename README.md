# Genesis Knowledge Packs

This repository publishes optional offline SQLite knowledge modules for the Android app **Genesis / 创世纪**.

The large knowledge databases are distributed only as GitHub Release assets. They are not committed to Git history and are not bundled in the APK. Larger assets use deterministic gzip transport; the app streams decompression directly into its private SQLite storage, verifies both the downloaded asset and the original database, and then uses the local FTS5 index for retrieval-assisted generation.

## Current release

- Tag: `knowledge-2026.03.05-r1`
- 13 logical knowledge modules
- 13 binary assets (4 SQLite assets and 9 gzip-compressed SQLite assets)
- Original installed payload: 6,322,401,280 bytes
- Total binary download payload: 4,113,463,323 bytes
- Catalog: `knowledge_pack_manifest.json`
- Asset checksums: `SHA256SUMS.txt`

## Integrity

The application catalog records the SHA-256 and exact byte size of each complete SQLite database. Gzip assets additionally carry the SHA-256 and exact byte size of the transferred compressed file. A module is not installed if the transfer, decompression, database metadata, or final SQLite integrity check fails.

## Sources and licenses

These are transformed search indexes made from offline source archives. See `THIRD_PARTY_NOTICES.md` and the metadata inside each SQLite database for source and license information. No endorsement by Wikipedia, Wikimedia, Kiwix, or Project Gutenberg is implied.

## Repository contents

Only documentation and machine-readable manifests are tracked here. Release binaries are attached to the corresponding GitHub Release.
