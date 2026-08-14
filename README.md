# Termy Dictionaries

Downloadable offline dictionary packs for [Termy](https://termy.lol/).

Each source-language pack is published as a gzip-compressed SQLite database in
[GitHub Releases](https://github.com/live-sound/Termy-Dictionaries/releases).
The database is unpacked locally by Termy and queried directly; the large pack
files are not stored in Git history.

## Available packs

| Source language | Content | Download | Installed | Release |
|---|---|---:|---:|---|
| English | English definitions, examples and forms; canonical translations into 29 supported languages | 200.1 MB | 480.4 MB | [`en-2026.08.12`](https://github.com/live-sound/Termy-Dictionaries/releases/tag/en-2026.08.12) |

The canonical machine-readable catalog is [`manifest.json`](manifest.json).
Clients should verify the asset's SHA-256 checksum before installation.

## Coverage

Translations are the canonical translations present in Wiktionary. They are not
a complete translation matrix: an entry or sense may have definitions but no
translation for the selected target language. Termy may use its online service
as a fallback for missing translations.

## License and attribution

The dictionary data is derived from English Wiktionary through the structured
Kaikki/Wiktextract export and is distributed under
[CC BY-SA 4.0](LICENSE). See [`NOTICE.md`](NOTICE.md) for attribution,
provenance, and the changes made during conversion.

This project is not affiliated with or endorsed by the Wikimedia Foundation,
Wiktionary, Kaikki.org, or Wiktextract.
