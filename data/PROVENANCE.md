# Provenance

Retrieved 2026-08-11 by `colab_pack/fetch_text_corpora.py`.

| Corpus | Source |
|---|---|
| MasakhaNEWS (AFL-3.0) | <https://github.com/masakhane-io/masakhane-news> |
| Project Gutenberg, via the ADH data reservoir (public domain) | <https://www.gutenberg.org/> |
| Internet Archive / open government (ECOWAS, ANC, TRC) | <https://archive.org/> |

## What was done

- **masakhanews.csv** — news documents with topic labels, capped per language (900 for the four Nigerian languages, 400 for the rest) and documents under 30 words dropped.
- **colonial_texts.csv / african_legal.csv** — each work split into ~220-word passages, evenly sampled to at most 40 per work so no single long book dominates the corpus.
- Project Gutenberg licence headers and footers stripped; leaving them in makes the boilerplate the most distinctive text in the corpus.

## Known limits

- The colonial-era corpus is a **colonial-discourse** collection, not African-authored. It comes from a Gutenberg keyword search for 'africa' and includes *Uncle Tom's Cabin* and an Agatha Christie novel. That is the point of the corpus, not a defect — but any claim from it is about how Africa was *written about*, in English, before 1929.
- MasakhaNEWS is news prose. Findings about it are about journalism, not about the languages in general.
- One ECOWAS report under CC BY-ND 4.0 was excluded: a no-derivatives licence does not permit redistributing the work split into sampled passages.
- Nothing here is in-copyright. Pirated novels staged elsewhere on this server are deliberately excluded and the build fails if one appears.

- `masakhanews.csv` — 8,400 rows, 9 columns
- `colonial_texts.csv` — 5,984 rows, 8 columns
- `african_legal.csv` — 1,692 rows, 8 columns
