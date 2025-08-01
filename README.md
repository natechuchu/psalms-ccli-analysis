# 🎵 Psalms & Worship Lyrics: A CCLI Analysis with NLP

This project explores the connection between modern worship music and the Book of Psalms by analyzing the top 100 CCLI Christian songs using Natural Language Processing (NLP) techniques. The goal is to uncover linguistic, emotional, and theological parallels between today's worship lyrics and the biblical Psalms.

## 📌 Table of Contents
- [Overview](#overview)
- [Objectives](#objectives)
- [Dataset](#dataset)
- [Methods](#methods)
  - [1. Sentiment Analysis](#1-sentiment-analysis)
  - [2. Named Entity Recognition](#2-named-entity-recognition)
  - [3. POS Tagging](#3-pos-tagging)
  - [4. Repetitiveness](#4-repetitiveness)
  - [5. Coreference Resolution](#5-coreference-resolution)
  - [6. Thematic Similarity](#6-thematic-similarity)
- [Findings](#findings)
- [Tech Stack](#tech-stack)
- [How to Run](#how-to-run)
- [Future Work](#future-work)
- [Acknowledgments](#acknowledgments)
- [Contact](#contact)

---

## 🧠 Overview

How closely do modern worship songs reflect the language, tone, and theology of the Psalms? I have always heard Christians criticize modern worship songs, yet they lacked an objective way to compare and contrast the linguistic structure between scripture and the songs.

To answer this, I used Stanford NLP and other Python tools to perform lexical and semantic analysis across the top 100 CCLI songs and compared them to the full text of the Psalms. This project is part of a submission to the Jerry Falwell Library Research Week competition. My team finsihed 3rd for the Theoretical category.

---

## 🎯 Objectives

- Identify which Psalms align most closely with modern worship songs
- Measure sentiment and emotional tones in lyrics vs. Psalms
- Explore repetition and grammatical structure in songwriting
- Analyze theological language patterns (e.g., use of names for God, themes of suffering, joy, justice)

---

## 📂 Dataset

- **Top 100 CCLI Worship Songs** (cleaned and formatted)
- **Book of Psalms** (KJV and NIV versions, depending on analysis)
- All text processed and stored in `.txt` or `.csv` format

---

## 🔬 Methods

### 1. 📈 Sentiment Analysis
- Used `TextBlob` and `VADER` to score the emotional tone of each lyric and psalm
- Compared distributions of positive/neutral/negative sentiment

### 2. 🧍 Named Entity Recognition
- Extracted theological references (e.g., “Jesus,” “Lord,” “King”) using SpaCy and Stanford NLP
- Tracked frequency and variety of divine names

### 3. ✍️ POS Tagging
- Analyzed grammatical structure across songs and Psalms
- Compared verb tense usage, pronoun choices (e.g., "I" vs. "You" in worship)

### 4. 🔁 Repetitiveness
- Measured word frequency, chorus reuse, and lexical redundancy in worship lyrics
- Compared to literary repetitiveness in Psalms (e.g., poetic parallelism)

### 5. 🔗 Coreference Resolution
- Resolved pronouns like “He,” “You,” and “His” to understand who is being referenced
- Useful for evaluating personal vs. communal tone

### 6. 🔍 Thematic Similarity
- Vectorized each song and psalm using `TF-IDF` and `cosine similarity`
- Matched each song to the top 3 most similar Psalms

---

## 📊 Findings

> **Sample insights:**
- 87% of songs showed closest similarity to Psalms of thanksgiving or praise
- Repetition in CCLI lyrics is 2.3x higher than in Psalms (on average)
- Songs heavily use second-person pronouns ("You") while Psalms more often balance between "I", "You", and "He"
- Sentiment in worship songs is overwhelmingly positive, whereas Psalms include a broader emotional spectrum

(See `/results` folder or `findings.pdf` for full report)

---

## 🛠 Tech Stack

- Python 3.10
- `pandas`, `nltk`, `spacy`, `textblob`, `scikit-learn`
- Stanford CoreNLP (via server)
- Jupyter Notebook
- Matplotlib / Seaborn (for visualization)

---

## 🏁 How to Run

1. Clone the repo:
```bash
git clone https://github.com/yourusername/psalms-ccli-nlp.git
cd psalms-ccli-nlp


