---
title: 'Inspicio: Open-Vocabulary, LLM-Based Sense Retrieval for Historical Languages'
authors:
- Michele Ciletti
date: '2026-09-01'
publishDate: '2026-10-19T13:58:38.400178Z'
publication_types:
- manuscript
publication: '*arXiv preprint arXiv:2609.00998*'
doi: 10.48550/arXiv.2609.00998
abstract: Word Sense Disambiguation has advanced rapidly for English and a handful
  of well-resourced modern languages, but it continues to assume the existence of
  a sense inventory and a word-to-sense mapping in the source language (Navigli, 2026).
  These assumptions break down for most historical and low-resource languages, whose
  dedicated WordNets are either incomplete or still under construction. We present
  Inspicio, an open-vocabulary retrieval pipeline that links tokens in context to
  synsets of the Open English WordNet (McCrae et al., 2020) without requiring any
  source-language inventory or mapping. For each occurrence, an instruction-tuned
  LLM produces two English translations of the surrounding sentence, a small set of
  candidate dictionary-style definitions, and a few candidate English lemmas. These
  outputs drive a hybrid retrieval step that combines dense definition-synset similarity,
  sparse lemma matching, and Maximal Marginal Relevance re-ranking. We evaluate the
  pipeline across a 6x6 grid of LLMs and sentence-embedding models on a new bilingual
  set of manually annotated Latin and Ancient Greek perception verbs, on a subset
  of PREMOVE dataset (Farina, 2025), and on a diachronic sample of Italian. The best
  configuration reaches 96% Recall@50 on the perception-verb test set, with each component
  contributing measurable gains, and remains competitive in the out-of-domain and
  cross-lingual settings.
links:
- name: arXiv
  url: https://arxiv.org/abs/2609.00998
---
