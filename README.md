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
  - [6. Lexical Analysis](#6-lexical-analysis)
- [Findings](#findings)
- [Tech Stack](#tech-stack)

---

## 🧠 Overview

How closely do modern worship songs reflect the language, tone, and theology of the Psalms? I have always heard Christians criticize modern worship songs, yet they lacked an objective way to compare and contrast the linguistic structure between scripture and the songs.

To answer this, I joined a team of four to use Stanford NLP and other Python tools to perform lexical and semantic analysis across the **top 100 CCLI songs** and compared them to the full text of **the Psalms**. This project is part of a submission to the Jerry Falwell Library Research Week competition, and my team placed **3rd** for the Textual/Investigative Undergraduate Poster.

---

## 🎯 Objectives

- Measure sentiment and emotional tones in lyrics vs. Psalms
- Explore repetition and grammatical structure in songwriting
- Analyze theological language patterns (e.g., use of names for God, themes of suffering, joy, justice)

---

## 📂 Dataset

- **Top 100 CCLI Worship Songs**
- **Book of Psalms** (ESV)
- All texts were processed and stored in `.txt` format. 

---

## 🔬 Methods
- Retrieved all the data and removed any unnecessary text (e.g., Song titles, Scripture Chapter headers)
- "Boiled" down the text using each method and output results in `.json` files
- Use Matplotlib, Seaborn, and other libraries to perform analysis
### 1. Sentiment Analysis
- Assess the emotional tone and diversity of sentiment in both datasets.

### 2. Named Entity Recognition
- Compare how often and in what way both the Psalms and CCLI songs refer to theological entities.

### 3. Parts of Speech Tagging
- Analyze the grammatical structure of lyrics to assess complexity and the roles of different parts of speech. 

### 4. Repetitiveness
- Identify repetitive phrases or concepts in both datasets. 

### 5. Coreference Resolution
- Explore how consistently both the Psalms and CCLI songs refer to God or theological entities, such as whether CCLI songs focus predominantly on personal or relational language (e.g., “You” or “He”) versus the formal references in the Psalms.

### 6. Lexical Analysis
- Compare the diversity and richness of vocabulary used in the Psalms versus CCLI songs

---

## 📊 Findings
We found that the Psalms have:
1) Higher lexical diversity
  - Lexical Analysis: On average, scripture had a higher text-to-token ratio
  - Part of Speech Tagging: The Psalms had a higher frequency of prepositions and punctuation, aligning with more formal clause-rich statements, while CCLI Songs focused more on Direct Personal Pronouns. 
2) A wider range of sentiments, including emotions such as fear and anger
  - Sentiment Analysis: Word clouds unveiled that songs employ more positive emotions such as love and grace, while scripture has a more balanced display of emotions, referencing the judgement and justice of God.
3) More references to God with richer descriptions of who he is
  - N-Grams Analysis: Modern songs tend to focus more on the individual experiences, while the Psalms direct the reader to God.
  - Coreference Resolution and Name Entity Recognition: Both methods showed that the Psalms explore more vivid attributes of God and historical references.
  
(See `Psalm-CCLI Analysis RW Poster.pdf` for full report)

---

## 🛠 Tech Stack

- Python 3.10
- Stanford CoreNLP 
- Jupyter Notebook
- Matplotlib / Seaborn 

---

