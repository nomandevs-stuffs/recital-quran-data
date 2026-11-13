# Attribution — duas/

- **Source repository:** https://github.com/fitrahive/dua-dhikr
- **Source data path:** `data/dua-dhikr/<category>/<lang>.json` (one JSON array per category per language; languages present in source: `id` Indonesian, `en` English)
- **License:** MIT License (see `LICENSE` in this folder, copied verbatim from the source repo on 2026-11-13)
- **Copyright:** Copyright (c) 2023 Fitrahive
- **Date copied:** 2026-11-13

## What was taken from the source (copied exactly, unaltered)

- The Arabic dua/dhikr text (`arabic`), including tashkeel.
- The English transliteration. **Note:** the source keeps a different transliteration per language file. The canonical `transliteration.en` in this folder was taken from the Indonesian (`id`) language file, which uses the diacritical style; the English language file's plain transliteration was not used. The two spellings of the same Arabic differ between the source's `en` and `id` files for all 97 entries — neither was corrected or normalized.
- The English `title`, `translation`, `notes`, `benefits`/`fawaid` (the source uses the key `benefits` in some English files and `fawaid` in others; both are mapped to `benefits` here) and the `reference` (the source's English `source` field, kept verbatim).
- Entry order and count (97 entries across 5 categories).

## What was created for this folder (NOT from the source)

- All Bangla (`bn`) content — `title.bn`, `translation.bn`, `transliteration.bn` (Arabic rendered in Bangla letters), `notes.bn`, `benefits.bn`, and the Bangla category names — was drafted for this folder and does not come from the source.
- The `source_type` field: `"quran"` only for entries whose source citation includes a Quran reference (`QS.`), otherwise `"hadith"`, or `"unknown"` when the source had no reference.

## What was deliberately NOT taken

- The Indonesian (`id`) translation, notes, and references were dropped per the Recital app's decision to ship only `en` and `bn`.
- No Bangla translation existed in the source; it was drafted (see above), not copied.

## Notes & known issues

- Indonesian-language source files were used only for the `latin` (transliteration) field, as noted above.
- The Arabic text in `evening-dhikr` #14 differs between the source's `en` and `id` files only in combining-mark order (NFC-equal, identical visible text); the English file's version was copied.
- The source contains one duplicated Arabic string in `daily-dua` (both occurrences of "Bismillah" before eating and before wudu — different titles and references); kept as in source.
- Religious references (`reference`) are copied verbatim from the source's English `source` field and may contain a mix of English and transliterated Indonesian phrasing (e.g. "dan", "HR. ...").

## Terms

The MIT License requires retaining the copyright notice and permission notice, both of which are preserved in `LICENSE` in this folder. The source repository URL is given above for reference and for reporting issues upstream.
