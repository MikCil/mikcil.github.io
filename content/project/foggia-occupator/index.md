---
title: Foggia Occupator Corpus (1945–1946)
date: 2025-06-07
links:
  - type: site
    url: https://github.com/MikCil/foggia_occupator
tags:
  - NLP
  - Corpora
  - Historical Research
  - Linguistic Resources
---

An openly licensed, machine‑readable corpus of the weekly newspaper The Foggia Occupator (Dec 1945–Aug 1946): 22 issues, 874 articles, and ≈216k words. It opens a compact window onto an “in‑between” phase of reconstruction in Southern Italy, where everyday life and military presence overlapped.

<!--more-->

The project turns a fragile local paper—printed by U.S. personnel and distributed across base and city—into a reusable resource for digital history, cultural analytics, and NLP. We processed high‑resolution scans with OCR, then used GPT‑4o–assisted correction followed by full human verification to produce clean text, segmented into article units with basic metadata. Building on the text, the accompanying research layers topics, named entities, and typed relations, and mines argumentative passages in civics‑ and conflict‑related content. Together, these enrichments enable network studies (the entity–relation graph spans 6,297 nodes and 9,094 edges) and discourse analyses (1,735 arguments, many implicit) that are hard to attempt with raw scans alone.

Early readings and measurements point to a clear temporal shift: coverage that initially leaned toward military operations and international news gradually gives way to local social life, culture, and community‑building. Columns like “Girl About Town,” “Nights ’Round Foggia,” and “Static from your AES” trace the city’s social rhythms and base culture, while special issues—most notably Christmas 1945—stage arguments about normalcy and conviviality through images and vignettes. Yet tensions surface, too: grain‑shortage protests and incidents in off‑limits bars remind us that coexistence was negotiated and sometimes strained. In the network, links between American personnel and Italian civic actors become denser over time, suggesting a growing—if uneven—integration.

We also piloted a retrieval‑augmented generation (RAG) pipeline on the corpus to test LLM‑assisted access to historical archives. Expert‑devised questions showed that tightly scoped prompts yield accurate, source‑grounded answers with solid entity resolution, while broader, multi‑article queries can produce partial or slightly erroneous outputs—evidence that better metadata, smarter retrieval weighting, and careful query strategy pay dividends.

The dataset is released under a Creative Commons Attribution 4.0 (CC BY 4.0) licence. The GitHub repository provides the JSON article collection; the paper describes additional releases (TEI‑XML with entity spans, CSVs for entities/relations with temporal counts, and an arguments JSON) to support reproducible cultural analytics and benchmarking. If you explore the corpus, I’d love to hear how you use it—whether for historical inquiry, discourse studies, or as a realistic testbed for OCR‑robust information extraction.
