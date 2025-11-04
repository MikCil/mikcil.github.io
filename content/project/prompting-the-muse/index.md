---
title: Veras Audire et Reddere Voces — Prosodically‑Accurate Latin Text-to-Speech Corpus and Methodology
date: 2025-07-26
tags:
  - Text-to-Speech
  - LLMs
  - Prosody
  - Latin
---

An openly licensed, expertly validated corpus of Latin poetic audio that makes classical metre audible with modern large‑language‑model TTS. Drawing on Pedecerto’s machine‑readable scansions, we steered a general‑purpose model to recite 216 lines—Vergil Aeneid 1.1–100 (hexameter) and Ovid Heroides 1.1–116 (elegiac couplets)—with metrically faithful stress, yielding nearly 24 minutes of line‑aligned, classroom‑ready audio. This project was presented at the ACL 2025 Student Research Workshop (Vienna) and at CLiC‑it 2025 (Cagliari).

<!--more-->

The workflow embraces a simple idea: encode prosody in the input. Each verse is syllabified, compulsory elisions are merged, caesurae are marked with commas, and every ictic syllable is upper‑cased with a grave accent on its vowel. A light orthographic adaptation (e.g., c→k before front vowels, qu→kw, ae/oe→ai/oi) nudges pronunciation away from English/Romance defaults. Fed to an LLM‑based TTS (gpt‑4o‑mini‑tts) via a compact prompt—“speak slowly, articulate every syllable, obey the visible stresses”—this representation reliably biases duration and emphasis without any model retraining. Ten takes per line are generated and screened by Latin phonology experts; at least one rendition met all criteria for the vast majority of verses, and accepted files were loudness‑normalised and concatenated with uniform verse pauses.

What emerges is both a teaching aid and a research test‑bed. Students can finally hear hexameter and pentameter as rhythm, not just as rules; instructors get aligned text–audio pairs for accessible pedagogy. For speech/NLP researchers, the bundle (Pedecerto XML, classical and TTS‑ready transcriptions, per‑line and stitched mp3) offers clean material for prosody control, few‑shot fine‑tuning, and quantitative metrics—complete with an error taxonomy (cross‑lingual accent drift, tricky clusters like ‑nx‑/tl‑, and length–stress trade‑offs) that suggests practical heuristics. Ablations show that case‑shift plus accent carry most of the gains, while syllable hyphenation adds little.

The corpus is released under CC BY 4.0 and accompanied by the scripts and prompts used to generate it, keeping replication straightforward with easily accessible APIs. Looking ahead, we aim to couple this prompt‑driven strategy with explicit duration control (FastSpeech‑type variance adapters), reduce best‑of‑N selection through lightweight alignment modules, broaden speakers and genres, and port the recipe to other metrical traditions (Ancient Greek, Classical Arabic). For now, it shows that—when prosodic knowledge is made visible—LLM‑TTS can make the dead speak rhythmically, reproducibly, and in the open.
