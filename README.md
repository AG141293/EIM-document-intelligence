# 🗂️ EIM Document Intelligence Engine

> Auto-Classification · PII Detection · Audit Trail · Semantic Search

[![Python](https://img.shields.io/badge/Python-3.10+-blue)](https://python.org)
[![Notebook](https://img.shields.io/badge/Platform-Google_Colab-orange)](https://colab.research.google.com)
[![Dataset](https://img.shields.io/badge/Dataset-UCI_News_Aggregator-green)](https://archive.ics.uci.edu/dataset/359)
[![License](https://img.shields.io/badge/License-MIT-lightgrey)](LICENSE)

---

## 📌 About

A Python end-to-end project inspired by the
[OpenText EIM Blueprint](https://opentext.com), demonstrating how
enterprise document management systems use AI/ML to:

- **Auto-classify** documents into Business / Technology /
  Entertainment / Medical categories
- **Detect and redact PII** (emails, phone numbers, SSNs,
  Aadhaar, PAN cards)
- **Maintain an immutable audit trail** using Python decorators
- **Search documents** with keyword matching

Built as a learning project covering **20+ core Python concepts**
in a single, real-world pipeline.

---

## 🗂️ Project Structure

```
eim-document-intelligence/
├── EIM_Document_Intelligence.ipynb   ← Main Colab notebook
├── README.md
└── LICENSE
```

---

## 🚀 Quick Start

1. Open the notebook in Google Colab:

   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/16nVQopYuTDtMcsGhTUJgQ6Zg0x_dfaBO?usp=sharing)

2. Run all cells — the dataset downloads automatically (~33 MB)

3. Expected runtime: ~3–5 minutes on Colab free tier

---

## 🧠 Python Concepts Covered

| Concept | Where Used |
|---|---|
| OOP — Classes, Inheritance, Properties | `Document`, `SensitiveDocument`, `EIMEngine` |
| Decorators | `@audit_log` for compliance trail |
| Generators | `document_stream()` batch processing |
| Regex (`re`) | PII detection engine |
| Exception Handling | `try/except` in PII scanner |
| List Comprehensions & Lambda | Feature engineering, search filter |
| `collections.Counter` / `defaultdict` | Frequency analysis, indexing |
| Type Hints | All function signatures |
| Pandas | EDA, feature engineering |
| Scikit-learn Pipeline | TF-IDF + ML classification |
| Matplotlib / Seaborn | 4 analytics charts |

---

## 📊 Dataset

**UCI News Aggregator** — 422,937 news headlines across 4 categories.

| Category | Label |
|---|---|
| Business | `b` |
| Technology | `t` |
| Entertainment | `e` |
| Medical / Health | `m` |

Downloaded automatically inside the notebook. No manual setup needed.

---

## 📈 Results

| Model | Accuracy |
|---|---|
| Logistic Regression (TF-IDF bigrams) | ~94–95% |
| Naive Bayes (TF-IDF bigrams) | ~91–93% |

---

## 🔧 Tech Stack

- Python 3.10+
- `pandas`, `numpy`, `scikit-learn`
- `matplotlib`, `seaborn`
- Google Colab (free)

---

## 📄 License

MIT — free to use, modify, and distribute.

---

> Inspired by the EIM Blueprint for building enterprise-grade
> document management systems as an OpenText alternative.
