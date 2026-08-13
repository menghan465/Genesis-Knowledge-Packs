# Genesis Knowledge Packs

This repository publishes optional offline SQLite knowledge modules for the Android app **Genesis / 创世纪**.

The large `.gknowledge.sqlite` files are distributed only as GitHub Release assets. They are not committed to Git history and are not bundled in the APK. The app downloads a selected module, validates its byte length and SHA-256 digest, and then uses its local FTS5 index for retrieval-assisted generation.

## Current release

- Tag: `knowledge-2026.03.05-r1`
- 13 logical knowledge modules
- 14 binary assets (the largest module is split into two ordered parts)
- Original installed payload: 6,322,401,280 bytes
- Catalog: `knowledge_pack_manifest.json`
- Asset checksums: `SHA256SUMS.txt`

## Integrity

The application catalog records the SHA-256 and exact byte size of each complete SQLite database. Split assets additionally carry per-part SHA-256 and size metadata. A module is not installed if any check fails.

## Sources and licenses

These are transformed search indexes made from offline source archives. See `THIRD_PARTY_NOTICES.md` and the metadata inside each SQLite database for source and license information. No endorsement by Wikipedia, Wikimedia, Kiwix, or Project Gutenberg is implied.

## Repository contents

Only documentation and machine-readable manifests are tracked here. Release binaries are attached to the corresponding GitHub Release.
