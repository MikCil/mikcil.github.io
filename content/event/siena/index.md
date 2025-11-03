---
title: "Prompting the Muse: Generating Prosodically-Correct Latin Speech with Large Language Models"
event: "AI and Digital Humanities: Methodological Approaches, Theories and Methods Conference"
event_url: "https://www.unisi.it/unisilife/eventi/ai-and-digital-humanities-methodological-approaches-theories-and-methods"

location: Università di Siena, Aula Magna storica
address:
  street: via Banchi di Sotto, 55
  city: Siena
  region: Toscana
  country: Italy

summary: """I will present a talk exploring how historical linguistics can partner with AI, presenting a case study on Latin prosody and the use of large language models to generate metrically correct speech. This presentation is part of the "AI and Digital Humanities" conference at the Università di Siena.
abstract: 'This study investigates whether prompt engineering, aided by symbolic prosodic markup, can induce a large language model-based text-to-speech (TTS) system to recite Latin verse with metrically correct stress. Two hundred dactylic lines - one hundred hexameters from Vergil's Aeneid and the opening elegiac couplet sequence of Ovid''s Heroides - were taken from the Pedecerto corpus, whose XML already encodes syllabification, ictus positions, and caesurae (Colombi et al., 2011). A preprocessing pipeline syllabified each verse, merged obligatory elisions, inserted commas at caesurae, transliterated graphemes toward an English-Italian compromise, upper-cased every ictic syllable, and placed a grave accent on its vowel. The verses were supplied to gpt-4o-mini-tts (Hurst et al., 2024), which resulted to be the best-performing model for the task, through a compact system prompt requesting slow, articulated speech that obeys the visible stresses. Ten stochastic realisations per line were generated; three independent Latin scholars evaluated the output, labelling segmental, stress, elision, and pacing errors. At least one recording met all criteria for 91% of the 216 lines. Ablation confirmed that case-shift plus accent carried most of the improvement, whereas syllable hyphenation was superfluous. Persistent errors clustered around lexical cognates whose default English or Romance stress conflicts with the metrical ictus. The present workflow achieves a promising prosodic fidelity while leveraging only text-level cues and the model''s general acoustic decoder, following an approach similar to the one outlined by Lam et al. (2025). It also sidesteps the scarcity of duration-marked training data that hampers quantitative reconstructions of Latin phonology (De Sisto et al., 2024). The resulting corpus, which consists of aligned text, validated audio, and scripts, will be openly released on Zenodo, supporting pedagogy, accessibility, and computational metrics research. Future work aims to couple the current strategy with controllable duration predictors offered by FastSpeech-type models (Ren et al., 2020) and train lightweight alignment modules to reduce the need for manual best-of-N selection, in line with broader calls for FAIR audio resources in Digital Humanities (De Sisto et al., 2024)."""

# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
date: '2025-11-05T11:30:00Z' # Your specific talk start time
date_end: '2025-11-05T12:30:00Z' # Approximate end of your panel
all_day: false

# Schedule page publish date (NOT talk date).
publishDate: '2024-05-30T00:00:00Z' # Set to current date

authors:
  - admin # Assuming your author ID is michele-ciletti

tags:
  - AI
  - Digital Humanities
  - Linguistics
  - Latin
  - Prosody
  - Text-to-Speech
  - Conference
  - Siena

# Is this a featured talk? (true/false)
featured: true

image:
  caption: 'Conference poster. Image credit: [**Università di Siena**](https://www.unisi.it/)'
  focal_point: Center

links:
  - type: program
    url: "https://www.unisi.it/unisilife/eventi/ai-and-digital-humanities-methodological-approaches-theories-and-methods" # Link to full conference program and online stream
  - type: video
    url: "https://shorturl.at/PXkMI" # Link to the online stream if available
  - type: slides
    url: '#' # Placeholder for your talk slides, update when available
  - type: code
    url: "https://zenodo.org/records/15677356" # Placeholder for Zenodo dataset/code release, update when available

# Markdown Slides (optional).
#   Associate this talk with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: ["prompting-the-muse"]
---

{{% callout note %}}
I am excited to be speaking at the **AI and Digital Humanities: Methodological Approaches, Theories and Methods Conference** at the University of Siena on November 4-5, 2025!
{{% /callout %}}

My presentation, **"Prompting the Muse: Generating Prosodically-Correct Latin Speech with Large Language Models"**, will take place on **November 5th** at **11:30 AM**. I will be part of the panel "Linguistic models and text interpretation" (chaired by Giancarlo Macchi) alongside other distinguished scholars. My talk explores how historical linguistics can partner with AI, presenting a case study on Latin prosody and the use of large language models for generating metrically correct speech, drawing from the research outlined in the abstract above.

The conference brings together an interdisciplinary group of scholars over two days to discuss the cutting-edge intersection of Artificial Intelligence and Digital Humanities. It will cover methodological approaches, theories, and tools, ranging from teaching and research to documentary heritage management and epistemological reflections.

Keynote speakers include:
*   **Giancarlo Macchi Jánica** (Università di Siena)
*   **Fabio Ciotti** (Università di Roma Tor Vergata)
*   **Frédéric Clavert** (Université du Luxembourg)

The program features various thematic panels covering topics such as:
*   AI in teaching the humanities
*   History, memory, and AI in digital contexts
*   AI and transparency in linguistic and historical analysis
*   AI and research tools and methods for humanities
*   Linguistic models and text interpretation
*   AI for document enhancement and use

Additionally, a round table titled "Publishers and AI" will explore the topic with representatives from Laterza and Carocci.

The full conference program, including details on how to follow the event online via streaming, is available through the **Program** link above.

The Scientific Committee coordinating this initiative is composed of: Elisabetta Bartoli, Fabio De Ninno, Emanuele Ertola, Michele Lacriola, Giancarlo Macchi Janica, Federico Mazzini, Deborah Paci, Enrica Salvatori, Francesco Stella, and Edmondo Trentin.
