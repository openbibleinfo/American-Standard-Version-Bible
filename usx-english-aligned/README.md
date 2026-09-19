# English alignment USX

This README is AI-generated.

These USX 3.0 files preserve the American Standard Version (1901) and add
word-level links to the accepted Greek, Hebrew, or Aramaic
alignment. For the same text without these extensions, use `../english-only/`.

Custom attributes use the `x-` prefix. Space-separated `*-ids` and `x-src`
values are ordered lists.

## Alignment attributes

On `<book>`:

- `x-source-language`: source language code (`grc`, `hbo`, or `arc`).
- `x-source-name`: display name of the source language.
- `x-source-dir`: source-script direction, `ltr` or `rtl`.

On `<char style="w">` (an ASV lexical token):

- `x-id`: token ID within the verse, normally `t001`, `t002`, and so on.
- `x-align`: stable ID of the alignment unit containing this token. All words
  on either side with the same value belong to the same unit.
- `x-status`: present when the unit is not an ordinary alignment: `added` for
  ASV wording with no source token, or `noncompositional` when the two sides
  correspond only as a whole.
- `x-head="true"`: this ASV token is the display head of its unit.
- `x-src`: source token IDs in the unit. It appears once, on the unit's display
  token.
- `x-source`: source forms corresponding to `x-src`, or `∅` for an `added`
  unit.
- `x-translit`: transliterations corresponding, in order, to `x-source`.
- `srcloc`: ID of the source head token.
- `lemma` and `strong`: lemma and Strong's identifier of that source head,
  when available.

On a verse milestone (or a descriptive-title paragraph representing verse 0):

- `x-unrepresented-src`, `x-unrepresented-source`, and
  `x-unrepresented-translit`: IDs, forms, and transliterations for source
  tokens that have no ASV wording.
- `x-supplied-from`: source reference used when this verse has no text at its
  expected location in the source edition.

## Supplementary footnote readings

Selected translated readings inside ASV notes use the same word attributes.
The containing `<note>` may also have:

- `x-footnote-id`: stable ID of the supplementary reading.
- `x-host-ref`: verse containing the note.
- `x-source-citation`: citation for the projected source reading.
- `x-source-projection`: short label for that projection.
- `x-projection-limitations`: known limits of the projection.
- `x-unrepresented-*`: source-only tokens in the supplementary reading, with
  the same meanings as above.

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
