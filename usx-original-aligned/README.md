# Original-language alignment USX

This README is AI-generated.

These USX 3.0 files present the accepted source projection in source order,
with links to the American Standard Version (1901). Greek, Hebrew, and Aramaic
tokens retain their spelling, spacing, parsing, and language metadata. Hebrew
prefixes and suffixes remain separate morpheme tokens; bracketed forms such as
`[הַ]` are real zero-letter morphemes represented by their supplied display
form.

Custom attributes use the `x-` prefix. Space-separated `*-ids` values are
ordered lists.

## Document and verse attributes

On `<book>`:

- `x-source-language`, `x-source-name`, and `x-source-dir`: source language
  code, display name, and script direction.
- `x-target-language="eng"` and `x-target-name`: identify the ASV target.
- `xml:lang`: language of the book text.

On a verse milestone (or a descriptive-title paragraph representing verse 0):

- `x-ref`: canonical alignment reference, such as `MAT.1.1`.
- `x-added-alignments`: IDs of units containing ASV words but no source token.
- `x-added-target-ids`: ASV token IDs in those units.
- `x-added-target`: their ASV text; separate units are divided by ` | `.

## Source-token attributes

Each `<char style="w">` is one source token or morpheme:

- `x-id`: stable source token ID.
- `x-align`: stable alignment-unit ID. Tokens on either side with the same
  value belong to the same unit.
- `x-status`: present when the unit is not ordinary: `unrepresented` for a
  source token with no ASV wording, or `noncompositional` when the two sides
  correspond only as a whole.
- `x-head="true"`: source head of the unit. Target metadata is stored on this
  token only.
- `x-target-ids`: ASV token IDs in the unit.
- `x-target`: the corresponding ASV text.
- `x-target-head`: ASV head-token ID.
- `x-target-italic-ids`: target IDs printed as supplied-word italics in the
  ASV.
- `lemma`, `strong`, `x-morph`, and `x-gloss`: lexical ID, Strong's identifier,
  morphology, and source gloss, when available.
- `x-translit`: display transliteration.
- `xml:lang`: token language; this distinguishes Aramaic spans in Hebrew books.
- `x-source-ref`: source-edition reference when it differs from the canonical
  verse reference.

## Supplementary footnote readings

A `<note>` containing an alternate source reading may carry `x-footnote-id`,
`x-host-ref`, `x-source-citation`, `x-source-projection`, and
`x-projection-limitations`. Target-only words within that reading use the same
`x-added-*` attributes described above. IDs inside supplements are qualified by
the footnote ID to keep them unique.

## Licensing and attribution

These files combine and modify the following sources by tokenizing them,
selecting documented source projections, and adding alignment markup.

- The American Standard Version Bible is public domain.
- The [SBL Greek New Testament](https://github.com/Faithlife/SBLGNT), copyright
  2010 by the Society of Biblical Literature and Logos Bible Software, is
  licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
- “MACULA Greek Linguistic Datasets, available at
  https://github.com/Clear-Bible/macula-greek/.” Copyright 2022–2024 by
  Biblica, Inc.; [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
- “MACULA Hebrew Linguistic Datasets, available at
  https://github.com/Clear-Bible/macula-hebrew/.” Copyright 2022–2024 by
  Biblica, Inc.; [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
- “Original work of the Open Scriptures Hebrew Bible available at
  https://github.com/openscriptures/morphhb.” Its lemma and morphology data
  are [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/); its
  Westminster Leningrad Codex text is public domain.
- Cherith Glosses for the Greek New Testament, by Andi Wu, copyright 2023 by
  Cherith Analytics, and Cherith Glosses for the Hebrew Old Testament, by Andi
  Wu, copyright 2022 by Cherith Analytics, are licensed under
  [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
