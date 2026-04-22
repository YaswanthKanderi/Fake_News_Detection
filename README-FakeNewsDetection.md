# 🔍 Fake News Detection — NLP & Machine Learning Classifier

<div align="center">

![Python](https://img.shields.io/badge/Python-3.8+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![NLTK](https://img.shields.io/badge/NLTK-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![Accuracy](https://img.shields.io/badge/Accuracy-95%2B%25-2ea44f?style=for-the-badge)

**A high-accuracy NLP pipeline to detect misinformation using classical machine learning.**

[📊 View Notebook](#-notebook) · [🚀 How It Works](#-how-it-works) · [📈 Results](#-results) · [🛠 Setup](#-setup)

</div>

---

## 📌 Overview

Fake news detection is a critical challenge in today's information ecosystem — and a direct analogue to threat intelligence problems in cybersecurity: classify signals, separate noise from truth, automate detection at scale.

This project implements a full **Natural Language Processing (NLP) pipeline** that ingests raw news text, preprocesses it, extracts statistical features, and classifies articles as **Real** or **Fake** using multiple ML models — achieving **95%+ accuracy**.

---

## 🧠 How It Works

```
Raw Text Input
     │
     ▼
┌─────────────────────┐
│  Text Preprocessing │  ← Tokenisation, Lowercasing, Stop-word Removal, Stemming (NLTK)
└─────────────────────┘
     │
     ▼
┌─────────────────────┐
│  Feature Extraction │  ← TF-IDF Vectorisation (Term Frequency-Inverse Document Frequency)
└─────────────────────┘
     │
     ▼
┌─────────────────────────────────┐
│  Model Training & Evaluation    │
│  ├── Logistic Regression        │
│  └── Random Forest Classifier   │
└─────────────────────────────────┘
     │
     ▼
  Prediction: REAL / FAKE
```

---

## 📈 Results

| Model | Accuracy | Precision | Recall | F1 Score |
|---|---|---|---|---|
| Logistic Regression | **95.2%** | 94.8% | 95.6% | 95.2% |
| Random Forest | **94.7%** | 94.1% | 95.3% | 94.7% |

> Both models were evaluated on an unseen test split to prevent data leakage.

---

## 🛠 Tech Stack

| Layer | Tools |
|---|---|
| Language | Python 3.8+ |
| NLP | NLTK (tokenisation, stemming, stop-word removal) |
| Feature Engineering | TF-IDF Vectorisation (scikit-learn) |
| Models | Logistic Regression, Random Forest |
| Evaluation | Accuracy, Precision, Recall, F1, Confusion Matrix |
| Notebook | Jupyter Notebook |

---

## 🔐 Security & Real-World Relevance

This project mirrors core techniques used in **cyber threat intelligence**:

- **Signal classification** — distinguishing legitimate vs malicious (fake) content at scale
- **Feature extraction from unstructured text** — applicable to log analysis and phishing detection
- **Automated decision pipelines** — reducing manual analyst workload
- **Model validation** — ensuring detection systems don't miss threats (high recall priority)

---

## 🚀 Setup & Run

```bash
# Clone the repo
git clone https://github.com/YaswanthKanderi/Fake_News_Detection.git
cd Fake_News_Detection

# Install dependencies
pip install -r requirements.txt

# Launch the notebook
jupyter notebook
```

### Dependencies
```
nltk
scikit-learn
pandas
numpy
matplotlib
seaborn
jupyter
```

---

## 📁 Project Structure

```
Fake_News_Detection/
├── Fake_News_Detection.ipynb   # Main notebook
├── dataset/
│   ├── True.csv                # Real news articles
│   └── Fake.csv                # Fake news articles
├── requirements.txt
└── README.md
```

---

## 👨‍💻 Author

**Yaswanth Kanderi**
Master of Cyber Security — La Trobe University, Melbourne

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/yaswanthkanderi/)
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/YaswanthKanderi)
[![Email](https://img.shields.io/badge/Email-0078D4?style=for-the-badge&logo=microsoft-outlook&logoColor=white)](mailto:yaswanthchowdary01@outlook.com)

---

<div align="center">
<i>"Detecting misinformation today — securing systems tomorrow."</i>
</div>
