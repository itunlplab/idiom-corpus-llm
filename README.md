# Using LLMs to Advance Idiom Corpus Construction

This repository contains the data and code for the paper "**Using LLMs to Advance Idiom Corpus Construction**," accepted at the 21st Workshop on Multiword Expressions (MWE 2025), co-located with NAACL 2025 in Albuquerque, New Mexico, U.S.A.

[Doğukan Arslan](https://web.itu.edu.tr/arsland15), [Hüseyin Anıl Çakmak](), [Gülşen Eryiğit](https://web.itu.edu.tr/gulsenc/), [Joakim Nivre](https://jnivre.github.io)

### 📝 TL;DR:
This research explores the use of large language models to generate synthetic idiom datasets and evaluate their effectiveness in training task-specific models for idiomaticity detection.

## 📂 Content
### ⚙️ Synthetic Data Generation
Python notebooks for synthetic data generation using GPT-4 in English, Italian, Japanese, and Turkish are available in this directory.
### 📑 Datasets
This directory contains datasets generated using GPT-4. For each language, sentences with potential idiomatic expressions (PIEs) are provided in separate CSV files, categorized based on their idiomatic (figurative) or literal usage. Each dataset includes the following columns:- `submission`: the sentence containing the potential idiomatic expression
- `submission`: synthetically generated sentence containing the PIE
- `category`: whether the PIE is used in its figurative (idiomatic) or literal sense
- `idiom`: the idiomatic expression in the sentence
- `type`: how the sentence is generated (e.g., zero-shot, enhanced-prompting)

Human-generated datasets that are used in the paper are available in the following links: [VNC-Token (English)](https://github.com/vasudev2020/BERTAnalysis/), [Dodiom (Italian)](https://github.com/Dodiom/dodiom/), [Open-MWE (Japanese)](https://github.com/nlp-waseda/OpenMWE/), [Dodiom (Turkish)](https://github.com/Dodiom/dodiom/).

### 📊 Evaluation
### Task 1: N-Shot Prompting
Code for evaluating GPT-4’s performance in idiomaticity  detection across various n-shot prompting settings, including zero-shot, one-shot, and few-shot scenarios, using both synthetic and human-generated data.
### Task 2: Task-Specific Fine-Tuning
Code for fine-tuning various BERT variants on the synthetic and human-generated data and evaluating their performance in idiomaticity detection.
### Task 3: Zero-Shot vs. Enhanced Prompting
Code for investigating the contributions of the two distinct prompting methods used for synthetic data generation.
### Task 4: Multilingual Idiomaticity Detection
Code for evaluating the performance of multilingual models in idiomaticity detection task.