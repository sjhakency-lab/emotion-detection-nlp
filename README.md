# emotion-detection-nlp
Emotion Detection NLP – A Natural Language Processing project that analyzes text and identifies emotions such as joy, sadness, anger, fear, and neutral feelings.
# A Hybrid NLP Framework for Text Emotion-Sentiment Classification

## Overview

This research proposes a hybrid multi-task Natural Language Processing (NLP) framework for jointly performing sentiment analysis and emotion classification on textual data.

Sentiment analysis identifies the overall polarity of text (positive, negative, or neutral), while emotion classification recognizes more specific emotional states such as joy, sadness, anger, fear, and other emotions.

The proposed framework uses a shared pretrained Transformer encoder with two task-specific classification heads and an optional lightweight linguistic feature component. The aim is to explore the balance between classification performance and computational efficiency.

## Objectives

- Develop a unified framework for sentiment and emotion classification.
- Compare independent task-specific models with a shared multi-task architecture.
- Investigate the contribution of additional linguistic features.
- Evaluate classification quality alongside computational cost.

## Proposed Methodology

The framework consists of four main components:

1. **Text Preprocessing** – Prepare and tokenize textual data while preserving meaningful linguistic information.
2. **Shared Transformer Encoder** – Extract contextual representations using a pretrained transformer such as DistilBERT.
3. **Linguistic Feature Extraction** – Optionally incorporate negation indicators, punctuation features, and sentiment-lexicon scores.
4. **Task-Specific Classification Heads** – Separate heads predict sentiment polarity and emotion categories.

## Model Configurations

| Model | Description |
|---|---|
| Model A | Independent transformer for sentiment classification |
| Model B | Independent transformer for emotion classification |
| Model C | Shared encoder with two task-specific heads |
| Model D | Model C with additional linguistic features |

## Candidate Datasets

- **GoEmotions** – Fine-grained emotion classification dataset.
- **TweetEval** – Benchmark containing a sentiment classification task.

The datasets provide different annotations, so the proposed framework uses task-specific training batches and masked loss computation rather than assuming both labels are available for every text.

## Evaluation Metrics

- Macro-averaged F1-score (primary metric)
- Precision
- Recall
- Accuracy
- Per-class evaluation and confusion matrices
- Trainable parameter count
- Model size
- Inference latency

## Research Status

This repository documents the proposed framework and experimental protocol.

**Experimental results are not yet available.** The models have not yet been trained or evaluated, and no performance scores are claimed at this stage.

## Limitations

- The candidate datasets differ in domain, label structure, and class distribution.
- Sentiment and emotion annotations are not paired for the same text across the selected datasets.
- Findings may not generalize to long-form text, other languages, or different domains.
- Computational efficiency must be verified through actual measurements.

## Future Work

- Implement and train the proposed configurations.
- Conduct experiments on GoEmotions and TweetEval.
- Compare performance across all four configurations.
- Analyze class-wise predictions and errors.
- Investigate paired sentiment-emotion datasets and improved multi-task learning methods.

## Technologies & Concepts

- Natural Language Processing (NLP)
- Transformer-based models
- Multi-task learning
- Sentiment analysis
- Emotion classification
- Hybrid text classification
- Computational efficiency

## Research Paper

The research paper associated with this project is available in this repository.

**Title:** A Hybrid NLP Framework for Text Emotion-Sentiment Classification: An Efficient Multi-Task Approach

## Author

**Kency Jha**  
B.Tech – Computer Science and Engineering  
Sharda University, Uttar Pradesh, India
