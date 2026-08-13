# Genesis Knowledge Packs

This repository publishes optional offline SQLite knowledge modules for the Android app **Genesis / 创世纪**.

The large knowledge databases are distributed only as GitHub Release assets. They are not committed to Git history and are not bundled in the APK. Larger assets use deterministic gzip transport; the largest gzip stream is divided into ordered parts for more reliable GitHub delivery. The app streams the downloaded bytes directly into gzip decompression, verifies every part, the complete gzip stream, and the resulting SQLite database, and then uses the local FTS5 index for retrieval-assisted generation.

## Current release

- Tag: `knowledge-2026.03.05-r1`
- 13 logical knowledge modules
- 15 binary assets: 4 complete SQLite assets, 8 single gzip assets, and 3 ordered parts belonging to the largest gzip stream
- Original installed payload: 6,322,401,280 bytes
- Total binary download payload: 4,113,463,323 bytes
- Catalog: `knowledge_pack_manifest.json`
- Asset checksums: `SHA256SUMS.txt`

## App installation flow

The APK contains the small core knowledge database and a catalog of the optional modules. In the app, the user chooses a module and taps download. No ZIM file, database path, URL, or checksum needs to be entered manually. Optional modules are downloaded from this repository's GitHub Release and installed into the application's private storage.

## Integrity

The application catalog records the SHA-256 and exact byte size of each complete SQLite database. Gzip assets additionally carry the SHA-256 and exact byte size of the complete compressed stream. Multipart downloads also record the SHA-256 and exact byte size of every ordered part. A module is not installed if a part, the complete transfer, decompression, database metadata, or final SQLite integrity check fails.

## Sources and licenses

These are transformed search indexes made from offline source archives. See `THIRD_PARTY_NOTICES.md` and the metadata inside each SQLite database for source and license information. No endorsement by Wikipedia, Wikimedia, Kiwix, or Project Gutenberg is implied.

## Repository contents

Only documentation and machine-readable manifests are tracked here. Release binaries are attached to the corresponding GitHub Release.
