# Attribution and provenance

The Termy dictionary packs distributed from this repository contain material
created by Wiktionary contributors. The native-edition packs in this catalog are:
English, German, French, Spanish, Italian, Portuguese, Vietnamese, Polish, Dutch, Czech, Turkish, Russian, Japanese, Chinese, Korean, Thai, Greek.

The following headword packs are derived from the English Wiktionary edition and
therefore contain English definitions: Swedish, Ukrainian, Hindi, Romanian, Hungarian, Danish, Norwegian Bokmål, Finnish, Croatian, Slovak, Belarusian, Bulgarian, Macedonian.

- Wiktionary: https://www.wiktionary.org/
- English Wiktionary: https://en.wiktionary.org/
- Contributor histories: available through each entry's history page
- Copyright information: https://en.wiktionary.org/wiki/Wiktionary:Copyrights
- Pack license: Creative Commons Attribution-ShareAlike 4.0 International,
  https://creativecommons.org/licenses/by-sa/4.0/

The structured exports were produced by **Wiktextract** and published by
**Kaikki.org**:

- Kaikki: https://kaikki.org/
- Wiktextract: https://github.com/tatuylonen/wiktextract

## Changes made by Termy

Termy converts the structured exports into compact SQLite databases optimized
for offline, case-insensitive lookup. The conversion:

- retains headwords, selected parts of speech, definitions, up to six examples
  per sense, inflected-form mappings, and canonical translations;
- removes inflection-only senses, empty records, source-parser metadata, and
  data not exposed by Termy's dictionary experience;
- deduplicates lemmas, definitions, forms, and translation surfaces;
- maps compatible language aliases such as `nb` to `no` and `sh` to `hr`;
- supplements safely matched entries with canonical translation links from the
  English pack without replacing definitions from the source edition;
- stores repeated values as integer identifiers and adds lookup indexes, pack
  metadata, and gzip compression.

These packs are adaptations distributed under CC BY-SA 4.0 and provided without
warranty. Termy is not affiliated with or endorsed by the Wikimedia Foundation,
Wiktionary, Kaikki.org, or Wiktextract. Each release's notes and `manifest.json`
identify its source, artifact sizes, checksums, and database schema version.
