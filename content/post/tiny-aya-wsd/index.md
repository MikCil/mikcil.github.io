---
title: "Cross-lingual Word Sense Disambiguation with Tiny Aya"
summary: "Our Expedition Tiny Aya project on multilingual Word Sense Disambiguation was featured on the Cohere blog."
date: 2026-07-15
authors:
  - admin
tags:
  - Word Sense Disambiguation
  - Multilingual NLP
  - Small Language Models
  - Datasets
  - Cohere
image:
  caption: "Image credit: [Cohere](https://cohere.com/blog/tiny-aya-in-the-wild)"
projects: ["tiny-aya-wsd"]
---

Cohere published a [blog post](https://cohere.com/blog/tiny-aya-in-the-wild) about the projects that came out of Expedition Tiny Aya, and the Word Sense Disambiguation project I have been leading since February is one of them!

Expedition Tiny Aya is a research program that Cohere Labs started shortly after releasing Tiny Aya, its open-weight multilingual model, to get the model into the hands of researchers, students and builders, with mentoring from Cohere. Our team was Alisa Banerjee, Hamza Shezad, Sirichada Wattanasiritanawong, Ahanaf Aziz and me, and our mentor was Ammar Khairi.

We wanted to find out how well a small multilingual model can learn to tell the senses of a word apart in many languages at once. Word Sense Disambiguation is the task of deciding which meaning a word has in a given sentence (I wrote about why it matters for Latin and Ancient Greek [in this post](/post/classical-semantics/)). Most of the research on it has been done in English, while the training and evaluation data for other languages is much smaller.

To train and test the models, we built a new version of XL-WSD (Pasini et al., 2021), a sense-annotated benchmark covering 18 languages, from Basque and Bulgarian to Japanese and Korean, and reformatted it as instruction data for language models. Every instance comes in two forms. In the multiple-choice version, the model reads the sentence and a numbered list of candidate definitions and answers with the number of the correct one; in the generation version, it gets only the sentence and the target word, and has to write the definition itself. We kept only definitions in the same language as the sentence and dropped words with a single sense, so that every example actually requires disambiguation. The dataset is [on Hugging Face](https://huggingface.co/datasets/MikCil/xlwsd-gloss-mcq) and follows the XL-WSD non-commercial license.

We then trained and evaluated Tiny Aya models across these languages. In the words of Cohere's summary, we observed strong cross-lingual transfer, "with some configurations achieving performance competitive with substantially larger models".

![Our project as described in Cohere's blog post](cohere-blog-wsd.png "Screenshot from [Tiny Aya in the wild](https://cohere.com/blog/tiny-aya-in-the-wild) on the Cohere blog")

Many thanks to my teammates, to Ammar for the mentoring, and to Cohere Labs for running the program.
