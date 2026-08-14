# Attribution and provenance

The Termy dictionary packs distributed from this repository contain material
derived from **English Wiktionary**, created by Wiktionary contributors.

- Original project: https://en.wiktionary.org/
- Contributor histories: available through the history page of each entry
- Copyright information: https://en.wiktionary.org/wiki/Wiktionary:Copyrights
- License used for these packs: Creative Commons Attribution-ShareAlike 4.0
  International, https://creativecommons.org/licenses/by-sa/4.0/

The structured source export was produced by **Wiktextract** and published by
**Kaikki.org**:

- Project: https://kaikki.org/
- English export: https://kaikki.org/dictionary/English/
- Wiktextract: https://github.com/tatuylonen/wiktextract

## Changes made by Termy

Termy converts the structured export into a compact SQLite database optimized
for offline, case-insensitive lookup. The conversion:

- retains English headwords, selected parts of speech, definitions, up to six
  examples per sense, inflected-form mappings, and canonical translations into
  Termy's supported languages;
- removes inflection-only senses, empty records, source-parser metadata, and
  data not exposed by Termy's dictionary experience;
- deduplicates lemmas, definitions, forms, and translation surfaces;
- stores repeated part-of-speech and language values as integer identifiers;
- combines multiple canonical translation surfaces for the same sense and
  target language; and
- adds SQLite lookup indexes, pack metadata, and gzip compression.

These packs are adaptations and are distributed under CC BY-SA 4.0. They are
provided without warranty. Termy is not affiliated with or endorsed by the
Wikimedia Foundation, Wiktionary, Kaikki.org, or Wiktextract.

Each release's notes and `manifest.json` identify the source snapshot, artifact
size, checksum, and database schema version.
