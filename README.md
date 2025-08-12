# Sentiment Analysis on Amazon Reviews using VADER and RoBERTa

# Project Overview

This project performs sentiment analysis on a dataset of Amazon product reviews using two popular approaches:

VADER (Valence Aware Dictionary and sEntiment Reasoner) – a rule-based NLP tool for sentiment classification.

RoBERTa – a pre-trained transformer-based deep learning model from Hugging Face, fine-tuned for sentiment analysis.

The goal is to compare the performance and contextual understanding of both models and demonstrate how modern NLP techniques outperform lexicon-based methods for nuanced customer feedback.

# Dataset Description

File: Reviews.csv

Contains thousands of Amazon customer reviews.

Key columns:

Text: The review content

Score: Star rating (used for ground-truth sentiment where applicable)

# Problem Statement

Can modern transformer-based models like RoBERTa offer more accurate and context-aware sentiment predictions than traditional rule-based tools like VADER?

# Methodology

Preprocessing

Cleaned text (lowercasing, removing special characters)

Removed or retained stop words depending on model requirements

Sentiment Modeling

VADER: Applied sentiment scoring (compound score → positive, neutral, negative)

RoBERTa: Used cardiffnlp/twitter-roberta-base-sentiment from Hugging Face Transformers

Comparative Evaluation

Converted predictions to common sentiment categories

Compared output distributions

Manually inspected sample cases where models disagreed

Visualization

Sentiment distribution bar charts

Word clouds and key phrase breakdowns

# Results & Insights

RoBERTa showed significantly better handling of sarcasm, negation, and context

VADER struggled with reviews that included subtle cues or complex syntax

For example: “This product works... when it wants to” was neutral in VADER but negative in RoBERTa

# Skills Demonstrated

Natural Language Processing (NLP)

Sentiment classification using rule-based and transformer models

Text preprocessing and tokenization

Use of Hugging Face Transformers and VADER lexicon

Visualization of sentiment results

# Project Files

Sentiment_Analysis_Cleaned.ipynb – Notebook comparing VADER and RoBERTa

Reviews.csv – Amazon reviews dataset

# How to Use

Install dependencies: transformers, vaderSentiment, pandas, matplotlib

Open the notebook and run all cells to reproduce sentiment scoring

Adjust thresholding or experiment with custom inputs

This project showcases how traditional and deep learning NLP models interpret user-generated content differently and can be applied in product feedback analysis or chatbot pipelines.


