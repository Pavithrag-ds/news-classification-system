# 📰 News Classification System

An End-to-End NLP and Machine Learning application that automatically classifies news articles into predefined categories such as **Business, Entertainment, Politics, Sports, Technology, and World News** using **TF-IDF Vectorization**, **Linear Support Vector Machine (Linear SVM)**, and **FastAPI**.

---

## 🚀 Project Overview

News articles are generated every minute across various domains. Automatically categorizing them helps improve content organization, recommendation systems, and information retrieval.

This project builds a complete NLP pipeline that preprocesses news articles, extracts textual features using TF-IDF, trains a Linear SVM classifier, and serves predictions through a FastAPI REST API.

---

## ✨ Features

- 📰 Automatic News Category Prediction
- 🧹 Text Cleaning and Preprocessing
- 📊 TF-IDF Feature Extraction
- 🤖 Linear Support Vector Machine (Linear SVM)
- ⚡ FastAPI REST API
- 📖 Swagger UI for API Testing
- 💾 Saved Trained Model & Vectorizer
- 🚀 Real-Time News Classification

---

## 🛠️ Tech Stack

### Programming Language

- Python

### Libraries

- Pandas
- NumPy
- NLTK
- Scikit-learn
- Joblib
- FastAPI
- Uvicorn

### Machine Learning

- TF-IDF Vectorizer
- Linear Support Vector Machine (Linear SVM)

### Development Tools

- VS Code
- Git
- GitHub

---

## 📂 Project Structure

```text
News_Classification
│
├── data
│   ├── raw
│   ├── processed
│   │   └── cleaned_news.csv
│   └── feeds
│
├── models
│   ├── news_model.pkl
│   └── tfidf_vectorizer.pkl
│
├── src
│   ├── api
│   │   └── app.py
│   ├── data
│   ├── features
│   ├── models
│   └── routing
│
├── main.py
├── requirements.txt
├── README.md
└── .gitignore
```

---

## ⚙️ Installation

### Clone Repository

```bash
git clone https://github.com/Pavithrag-ds/news-classification-system.git
```

```bash
cd news-classification-system
```

### Create Virtual Environment

```bash
python -m venv .venv
```

### Activate Virtual Environment

Windows

```bash
.venv\Scripts\activate
```

Linux / Mac

```bash
source .venv/bin/activate
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

---

## 🚀 Run the FastAPI Application

```bash
uvicorn src.api.app:app --reload
```

Open your browser:

```
http://127.0.0.1:8000/docs
```

Swagger UI will be available for testing the API.

---

## 📡 API Endpoint

### POST `/predict`

### Request

```json
{
  "text": "India wins the cricket world cup after an exciting final."
}
```

### Response

```json
{
  "category": "sports"
}
```

---

## 🧠 Machine Learning Pipeline

```
News Article
      │
      ▼
Text Preprocessing
      │
      ▼
TF-IDF Vectorization
      │
      ▼
Linear SVM Model
      │
      ▼
News Category Prediction
```

---

## 📊 Model Workflow

- Data Collection
- Data Cleaning
- Text Preprocessing
- Feature Engineering (TF-IDF)
- Model Training
- Model Evaluation
- Model Serialization
- FastAPI Development
- Real-Time News Classification

---

## 🏷️ News Categories

The model classifies news articles into the following categories:

- Business
- Entertainment
- Politics
- Science
- Sports
- Technology
- World

---

## 📦 Dataset

This project uses the **Inshort News Dataset** for training and evaluation.

The original dataset is not included in this repository due to its size. Download the dataset separately and place it inside the `data/raw/` directory before running the preprocessing pipeline.

---

## 👨‍💻 Author

**Pavithra G**

---

## ⭐ If you found this project useful

Please consider giving this repository a ⭐ on GitHub.