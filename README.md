<!-- BEGIN GENERATED -->
# Computational Text Analysis Pack

Computational text analysis for African digital humanities. One notebook per
method, where **one row is a document, a passage or a word** rather than a
spreadsheet cell. Built for scholars of literature, languages and linguistics
who want the statistics behind the tools.

## Using them

Each notebook is self-contained — open any one without having run the others.

**In Google Colab:** click the badge at the top of a notebook, then run the
first cell. It will ask you to upload the CSVs; pick them from this pack's
`data/` folder. The upload is remembered for the rest of the session.

**Locally:** put the notebook in the same folder as the CSVs and run it.
Needs `pandas`, `numpy`, `matplotlib`, `scipy`, `scikit-learn`, `statsmodels`.

**Inside CourseHub:** every notebook is also the 📓 Lab Notebook tab on its
lesson, next to the quiz. Nothing to install and no upload step.

## Data

Real African-language and African-archive text. News in 16 African languages
with topic labels, passages from 150 public-domain works about Africa, and
passages from 48 African court judgments and government reports.
Everything is public domain, open government, or AFL-3.0. Nothing in-copyright
is included. See `data/PROVENANCE.md`.

| File | What it is |
|---|---|
| `masakhanews.csv` | news in 16 African languages with topic labels; 3,600 of the 8,400 documents are in Hausa, Igbo, Yoruba or Nigerian Pidgin |
| `colonial_texts.csv` | 5,984 passages from 150 public-domain works about Africa — a colonial-discourse corpus, not an African-authored one |
| `african_legal.csv` | 1,692 passages from 48 African court judgments and government reports |

## The notebooks

| # | Notebook | Technique |
|---|---|---|
| | **Module 00 — Text as Data** | |
| `00` | [Text as Data](notebooks/00_text_as_data.ipynb) | Turning a corpus into a table: document, token, type |
| | **Module 01 — Framing the Question** | |
| `01a` | [What a Corpus Can and Cannot Answer](notebooks/01a_what_a_corpus_answers.ipynb) | Matching a literary or linguistic question to a countable method |
| `01b` | [Whose Africa Is in the Public Domain?](notebooks/01b_whose_africa_is_public_domain.ipynb) | Corpus construction as an argument; the absence audit for text |
| | **Module 02 — Describing a Corpus** | |
| `02a` | [Word Frequency](notebooks/02a_word_frequency.ipynb) | Frequency distributions; raw counts vs normalised rates |
| `02b` | [Zipf's Law](notebooks/02b_zipfs_law.ipynb) | Rank-frequency distributions; the long tail and what it costs you |
| `02c` | [Type/Token Ratio and Its Trap](notebooks/02c_type_token_ratio.ipynb) | Vocabulary richness; length dependence and standardised TTR |
| `02d` | [Document Length as Evidence](notebooks/02d_document_length.ipynb) | Distributions of length; median vs mean; when a skew is the finding |
| | **Module 03 — Preparing Text** | |
| `03a` | [Stopwords Are Not Universal](notebooks/03a_stopwords_are_not_universal.ipynb) | Stopword removal; why English lists do nothing to African languages |
| `03b` | [Diacritics and the ASCII Trap](notebooks/03b_diacritics_and_the_ascii_trap.ipynb) | Unicode-aware tokenising; measuring what naive cleaning destroys |
| | **Module 04 — Comparing Corpora** | |
| `04a` | [Keyness: Which Words Distinguish a Corpus](notebooks/04a_keyness.ipynb) | Log-likelihood keyness; target vs reference corpus |
| `04b` | [Effect Size for Words](notebooks/04b_effect_size_for_words.ipynb) | Why significance is not importance; log ratio and %DIFF |
| `04c` | [Comparing Across Archives](notebooks/04c_comparing_across_archives.ipynb) | Keyness between unlike corpora; confounds you cannot remove |
| | **Module 05 — Concordance and Collocation** | |
| `05a` | [KWIC: Reading What a Count Points At](notebooks/05a_kwic_concordance.ipynb) | Keyword-in-context; using a count to direct close reading |
| `05b` | [Collocation: The Company a Word Keeps](notebooks/05b_collocation.ipynb) | Window co-occurrence; span and its effect on results |
| `05c` | [Association Measures: PMI, Dice and Log-Likelihood](notebooks/05c_association_measures.ipynb) | Choosing an association statistic and knowing what it favours |
| | **Module 06 — Clustering Documents** | |
| `06a` | [Vectorising Text: TF-IDF](notebooks/06a_vectorising_text.ipynb) | Document–term matrices; term weighting and what min_df does |
| `06b` | [Clustering Documents with K-Means](notebooks/06b_clustering_documents.ipynb) | K-means on TF-IDF; choosing k and reading clusters honestly |
| `06c` | [Dendrograms: Clustering Without Choosing K](notebooks/06c_dendrograms.ipynb) | Hierarchical clustering; linkage choice and cutting the tree |
| | **Module 07 — Classification** | |
| `07a` | [Train and Test: The Split That Makes a Number Mean Something](notebooks/07a_train_test_on_text.ipynb) | Held-out evaluation; leakage; the majority-class baseline |
| `07b` | [Features and Models: What Actually Moves the Number](notebooks/07b_features_and_models.ipynb) | Comparing feature settings and classifiers; cross-validation |
| `07c` | [Which Words Carry the Decision](notebooks/07c_which_words_carry_the_decision.ipynb) | Model coefficients as evidence; interpreting a linear classifier |
| | **Module 08 — Topic Modelling** | |
| `08a` | [Topic Modelling with LDA](notebooks/08a_topic_modelling_lda.ipynb) | Latent Dirichlet Allocation; documents as mixtures of topics |
| `08b` | [NMF: The Other Topic Model](notebooks/08b_nmf_topics.ipynb) | Non-negative matrix factorisation; comparing two models on one corpus |
| `08c` | [Reading Topics Sceptically](notebooks/08c_reading_topics_sceptically.ipynb) | Choosing k; coherence; the topics that are artefacts |
| | **Module 09 — Stylometry** | |
| `09a` | [Most-Frequent Words: The Signal Everyone Discards](notebooks/09a_most_frequent_words.ipynb) | MFW feature sets; why function words identify authors |
| `09b` | [Burrows's Delta](notebooks/09b_burrows_delta.ipynb) | Z-scored MFW plus a distance measure; the standard attribution method |
| `09c` | [Style Beyond Authorship](notebooks/09c_style_beyond_authorship.ipynb) | Stylometric features for genre, register and translation |
| | **Module 10 — Visualising Text** | |
| `10a` | [Charting Frequency and Difference](notebooks/10a_charting_frequency.ipynb) | Bar charts, ranked comparisons, and the axis decisions that mislead |
| `10b` | [Why Word Clouds Mislead](notebooks/10b_why_word_clouds_mislead.ipynb) | Diagnosing a visualisation; area perception and the alternatives |
| `10c` | [Dispersion: Where in a Text a Word Appears](notebooks/10c_dispersion_and_structure.ipynb) | Dispersion plots; distinguishing sustained themes from single episodes |
| | **Module 11 — From Counts to Argument** | |
| `11a` | [From Counts to Argument](notebooks/11a_from_counts_to_argument.ipynb) | Classifying what a number can carry: description, comparison, claim |
| `11b` | [What Frequency Cannot Show](notebooks/11b_what_frequency_cannot_show.ipynb) | The limits section; silence, negation, and who is absent |
| | **Module 12 — Capstone** | |
| `12` | [Capstone: A Complete Analysis](notebooks/12_capstone.ipynb) | The whole workflow, on a corpus and question of your own |

## Rebuilding

Notebooks are generated from `colab_pack/` in the coursehub repo.
Edit the content modules there, not the `.ipynb` files:

```bash
python colab_pack/build_pack.py --pack text --check --zip
```

Every notebook is executed end to end as part of the build, so the worked
answers are known to reproduce the figures quoted in the course.

<!-- END GENERATED -->
