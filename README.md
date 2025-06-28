# Sentiment Analysis on Amazon Product Reviews

This project compares two sentiment analysis models — **VADER** (lexicon-based) and **RoBERTa** (transformer-based) — on a dataset of Amazon product reviews. The objective is to evaluate how well each model's sentiment predictions align with actual user-assigned star ratings.

---

## Dataset

- Source: [Amazon Product Reviews](https://www.kaggle.com/datasets)
- Fields used: `Text`, `Score` (1–5 star ratings)
- Sample size: (500-2) reviews

---

## Models Compared

| Model     | Type          | Description |
|-----------|---------------|-------------|
| VADER     | Rule-based    | Uses a predefined sentiment lexicon |
| RoBERTa   | Transformer   | Fine-tuned deep learning model for sentiment classification |

---

## Results Summary

| Metric                      | VADER     | RoBERTa   |
|----------------------------|-----------|-----------|
| Accuracy                   | 83.1%     | **85.5%** |
| Correlation with Ratings   | 0.535     | **0.775** |

- **RoBERTa outperforms VADER** in both classification accuracy and correlation with ground truth.
- VADER is fast but struggles with neutral/negative sentiment.
- RoBERTa captures context and sentiment nuance much better.

---

