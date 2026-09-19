# American Standard Version Bible (1901)

This project contains the complete text of the 1901 American Standard Version Bible, including paragraphs and footnotes.

It also contains the ASV text with markup aligning the English to the original languages, as well as a hypothetical reconstruction of the eclectic original-language text used by the translators, tagged to the English. This markup allows you to create interlinear views of the ASV, among other uses. Learn more about the alignment at the [companion project](https://github.com/openbibleinfo/American-Standard-Version-Bible-Alignment-Data).

## Purpose

The primary purpose of this project is to provide a high-fidelity digital edition of the ASV.

The original-language alignment demonstrates [how AI can create an interlinear](https://www.openbible.info/blog/2026/09/asv-interlinear/).

### Footnotes

Footnotes contain the following changes from the original:

1. Non-book abbreviations are spelled out (e.g., "cp." becomes "compare").
2. Roman numerals ("Ps. xxiii") in passage references are Arabic ("Ps. 23") and follow modern punctuation standards ("Ps. 23:1").
3. In some footnotes, an em space was used to separate clauses. These files instead use a period (".").

## Format

The files are in [USX 3.0](https://ubsicap.github.io/usx/) format, which is an XML derivative of the [USFM](https://paratext.org/usfm/) format used by [United Bible Societies](https://www.unitedbiblesocieties.org/) and the [Digital Bible Library](https://library.bible/).

## Corrections

Corrections are welcome. If you've found an error, please compare your correction to scans of the [original print edition](https://archive.org/details/holybible00newy), which is what I aim to reproduce.

As red-letter text (marking the words of Christ in red) isn't a feature of the ASV, I'm not interested in adding that markup to the text. Red-letter text occasionally requires some interpretation (as in John 3), which the original translation team didn't provide.

## Sources

In addition to PDFs of the source texts, the following digital editions were consulted:

- [STEP Bible](https://www.stepbible.org/?q=version=ASV|reference=Gen.1)
- [eBible](http://ebible.org/asv/)
- [Bible Gateway](https://www.biblegateway.com/versions/American-Standard-Version-ASV-Bible/)
- [CCEL](http://www.ccel.org/ccel/bible/asv.html)

## History of the ASV

The ASV Bible, published in 1901, was the first revision of the King James Version of 1611 to gain fairly widespread acceptance in the United States. It also served as the source text for the later RSV (followed by NRSV and ESV) and NASB translations.

## Interlinear Alignment

The alignment between the English and the Hebrew and Greek appears in the following folders. Each folder has a readme that explains the custom attributes.

- [usx-english-aligned](usx-english-aligned/) has the English as the base text and tags indicating the original-language words that are aligned to it.
- [usx-original-aligned](usx-original-aligned/) presents the Hebrew and Greek as the base text, tagged to the English. The source text attempts to present the eclectic text that the translators appear to have used, based on their translation choices.

An AI created this alignment over six weeks. It attempted to align as much of the English as possible with the original-language text, even where the ASV translators indicated that a word was added.

Read [more detail about the alignment](https://www.openbible.info/blog/2026/09/asv-interlinear/). The [companion repo](https://github.com/openbibleinfo/American-Standard-Version-Bible-Alignment-Data) goes into much more depth on alignment decisions.

## License: ASV Text

The ASV (English-only) text is free of known copyright restrictions. It is in the public domain.

[![Public Domain Mark](https://i.creativecommons.org/p/mark/1.0/88x31.png)](https://creativecommons.org/publicdomain/mark/1.0/)

## License: Interlinear Alignment

The alignment is based on CC-BY-4.0 sources and therefore carry that license, though the English text itself is in the public domain. Below are the credits. Also see [LICENSE.md](LICENSE.md).

- The [SBL Greek New Testament](https://github.com/Faithlife/SBLGNT), copyright 2010 by the Society of Biblical Literature and Logos Bible Software, is licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
- “MACULA Greek Linguistic Datasets, available at [https://github.com/Clear-Bible/macula-greek/](https://github.com/Clear-Bible/macula-greek/).” Copyright 2022–2024 by Biblica, Inc.; [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
- “MACULA Hebrew Linguistic Datasets, available at [https://github.com/Clear-Bible/macula-hebrew/](https://github.com/Clear-Bible/macula-hebrew/).” Copyright 2022–2024 by Biblica, Inc.; [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
- “Original work of the Open Scriptures Hebrew Bible available at [https://github.com/openscriptures/morphhb](https://github.com/openscriptures/morphhb).” Its lemma and morphology data are [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/); its Westminster Leningrad Codex text is public domain.
- Cherith Glosses for the Greek New Testament, by Andi Wu, copyright 2023 by Cherith Analytics, and Cherith Glosses for the Hebrew Old Testament, by Andi Wu, copyright 2022 by Cherith Analytics, are licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
