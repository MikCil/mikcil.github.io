---
title: Cross-Lingual Word Sense Disambiguation with Tiny Aya
date: 2026-07-15
links:
  - type: dataset
    url: https://huggingface.co/datasets/MikCil/xlwsd-gloss-mcq
  - type: site
    url: https://cohere.com/blog/tiny-aya-in-the-wild
tags:
  - Word Sense Disambiguation
  - Multilingual NLP
  - Small Language Models
  - Datasets
---

A project of Expedition Tiny Aya, the research program run by Cohere Labs around its open-weight multilingual model Tiny Aya. I led a team (Alisa Banerjee, Hamza Shezad, Sirichada Wattanasiritanawong, Ahanaf Aziz and me, mentored by Ammar Khairi) that trained and evaluated Tiny Aya models on Word Sense Disambiguation in 18 languages.

<!--more-->

Word Sense Disambiguation asks a model to decide which meaning a word has in context. For most languages other than English, sense-annotated data is scarce, which makes cross-lingual transfer an important question: can a small multilingual model learn the task in some languages and apply it in others?

To find out, we adapted XL-WSD (Pasini et al., 2021), a sense-annotated benchmark in 18 languages, into instruction data for language models. Each instance has two views that share the same gold sense: a multiple-choice question, where the model picks the correct definition from a numbered list, and a generation task, where it writes the definition without seeing any candidates. Candidate definitions are always in the language of the sentence, and words with a single sense are removed, so every example requires disambiguation. The resulting dataset, with train, dev and test splits, is released on [Hugging Face](https://huggingface.co/datasets/MikCil/xlwsd-gloss-mcq) under the XL-WSD non-commercial license.

The project was featured in Cohere's blog post [Tiny Aya in the wild](https://cohere.com/blog/tiny-aya-in-the-wild), which reports that the team observed strong cross-lingual transfer, with some configurations competitive with substantially larger models. More details are in [this blog post](/post/tiny-aya-wsd/).
