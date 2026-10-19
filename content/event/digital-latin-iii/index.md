---
title: "LLM-Driven, Open-Vocabulary Word Sense Disambiguation for Latin Digital Lexicography"
event: "Digital Latin III: International Workshop on Digital Tools and AI for Research on the Latin Lexicon"
event_url: "https://centroideugsu.unisi.it/2026/03/05/digital-latin-iii/"

location: Santa Chiara Lab, Università di Siena
address:
  street: via di Valmontone, 1
  city: Siena
  region: Toscana
  country: Italy

summary: 'I presented Inspicio, an LLM-based pipeline that retrieves Open English WordNet senses for Latin words without a predefined list of candidates, at the third Digital Latin workshop in Siena.'
abstract: >-
  Word-Sense Disambiguation remains a central challenge in computational linguistics, and the task becomes particularly relevant for historical and low-resource languages, where comprehensive lexical resources are often incomplete or unavailable. This project introduces Inspicio, a language-agnostic, LLM-based framework for open-vocabulary disambiguation that bypasses predefined candidate lists by retrieving synsets from the Open English Wordnet, and evaluates it through a case study on Latin verbs. The approach investigates whether target words in a historical language can be mapped effectively to a large English-based semantic network, and how hybrid retrieval can manage the extreme granularity of Wordnet while preserving genuinely distinct meanings.

  The pipeline begins by generating two English translations of each Latin target sentence, one literal and one natural. Using these translations together with the original sentence, the model proposes candidate English substitute lemmas and dictionary-style glosses for the target word, ordered by likelihood and able to represent multiple literal or metaphorical interpretations. All verb synsets in the Open English Wordnet are embedded by combining glosses, examples, lemmas, hypernyms, and lexnames. Retrieval combines dense cosine similarity with sparse lemma matching, boosts synsets supported by multiple retrieval signals, and applies a soft Maximal Marginal Relevance filter to avoid burying alternative meanings beneath minor variants of the dominant sense. The system outputs a top-k candidate pool. Preliminary experiments on Latin perception verbs and selected LatinISE data show promising results, with Recall@20 reaching 90% under the most effective combination of LLM and embedding model. Future work will aim to add an LLM reranker, broaden evaluation beyond verbs, test smaller open-weight models, and adapt the framework to other historical languages.

# Talk start and end times.
date: '2026-06-16T12:10:00Z'
date_end: '2026-06-16T12:30:00Z'
all_day: false

# Schedule page publish date (NOT talk date).
publishDate: '2026-06-16T00:00:00Z'

authors:
  - admin

tags:
  - Word Sense Disambiguation
  - Latin
  - Lexicography
  - LLMs
  - Conference
  - Siena

featured: false

image:
  caption: 'Title slide of the talk'
  focal_point: Center

links:
  - name: Program
    url: "https://centroideugsu.unisi.it/2026/03/05/digital-latin-iii/"
  - type: code
    url: "https://github.com/MikCil/inspicio"
  - type: preprint
    url: "https://arxiv.org/abs/2609.00998"

slides: ""

projects: []
---

My talk was part of the second day of the workshop, "Intelligenza artificiale e lingua latina". The workshop was organised by the Centro di Studi Comparati I Deug-Su and the Department of Philology and Criticism of Ancient and Modern Literatures of the University of Siena.

I presented an early version of Inspicio, the pipeline later described in my [arXiv preprint](https://arxiv.org/abs/2609.00998). The code is [on GitHub](https://github.com/MikCil/inspicio), and the proceedings of the workshop are in preparation.

I also wrote a [short post](/post/digital-latin-iii/) about the workshop.
