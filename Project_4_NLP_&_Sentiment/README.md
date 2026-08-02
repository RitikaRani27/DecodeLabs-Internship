# 🎬 NLP Sentiment Analysis using Machine Learning

A complete Natural Language Processing (NLP) project that classifies IMDB movie reviews as **Positive** or **Negative** using Machine Learning techniques. This project demonstrates the complete NLP pipeline from raw text preprocessing to model deployment.

---

## 📌 Project Overview

The objective of this project is to build a machine learning model capable of understanding and classifying human sentiment from movie reviews.

The project includes:

- Exploratory Data Analysis (EDA)
- Text preprocessing
- TF-IDF feature extraction
- Machine Learning model training
- Model evaluation
- Sentiment prediction on new reviews
- Model serialization for future use

This project was completed as part of the **DecodeLabs Machine Learning Internship (Project 4 – NLP & Sentiment Analysis)**.

---

# Dataset

**Dataset:** IMDB Movie Reviews Dataset

- 50,000 movie reviews
- Binary sentiment classification
- Balanced dataset
- Labels:
  - Positive
  - Negative

The size of dataset is too large so here's the link for dataset.
Dataset Source:
https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews

---

# Technologies Used

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn
- NLTK
- Scikit-Learn
- Joblib

---

# Project Workflow

## 1. Data Loading

- Import dataset
- Check data types
- Check missing values
- Remove duplicate reviews

---

## 2. Exploratory Data Analysis (EDA)

Performed:

- Sentiment distribution
- Review length analysis
- Word count analysis
- Duplicate review detection

---

## 3. Text Preprocessing

A complete NLP preprocessing pipeline was built including:

- Lowercasing
- HTML tag removal
- URL removal
- Removing punctuation
- Removing numbers
- Tokenization
- Stop-word removal
- Lemmatization

---

## 4. Feature Extraction

Reviews were converted into numerical vectors using:

**TF-IDF (Term Frequency–Inverse Document Frequency)**

Parameters used:

- max_features = 5000

---

## 5. Train-Test Split

- Training Data: 80%
- Testing Data: 20%

---

## 6. Machine Learning Models

Two classification models were trained:

- Multinomial Naive Bayes
- Linear Support Vector Machine (Linear SVM)

---

## 7. Model Evaluation

Models were evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix

---

# Results

| Model | Accuracy | Precision | Recall | F1 Score |
|--------|----------|-----------|--------|----------|
| Naive Bayes | **85.09%** | 84.76% | 85.69% | 85.22% |
| **Linear SVM** | **87.67%** | **87.54%** | **87.94%** | **87.74%** |

### Best Model

🏆 **Linear Support Vector Machine (Linear SVM)**

It achieved the highest performance across all evaluation metrics and was selected as the final model.

---

# Project Structure

```
NLP-Sentiment-Analysis/
│
├── Project4_NLP_Sentiment_Analysis.ipynb
├── sentiment_model.pkl
├── tfidf_vectorizer.pkl
├── README.md
└── requirements.txt
```

---

# Sample Predictions

| Review | Prediction |
|---------|------------|
| This movie was amazing. | Positive 😊 |
| Worst movie ever. | Negative 😞 |
| Excellent acting and story. | Positive 😊 |
| I regret watching this movie. | Negative 😞 |

---

# How to Run

### Clone Repository

```bash
git clone https://github.com/yourusername/NLP-Sentiment-Analysis.git
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Open

Run:

```
Project4_NLP_Sentiment_Analysis.ipynb
```

using

- Google Colab
- Jupyter Notebook

---

# Saved Models

The project saves:

- sentiment_model.pkl
- tfidf_vectorizer.pkl

These files can be loaded later for predicting sentiments of new reviews without retraining the model.

---

# Skills Demonstrated

- Natural Language Processing (NLP)
- Text Cleaning
- Tokenization
- Stop-word Removal
- Lemmatization
- TF-IDF Vectorization
- Feature Engineering
- Machine Learning Classification
- Naive Bayes
- Support Vector Machine (SVM)
- Model Evaluation
- Model Serialization
- Python Programming
- Data Visualization

---

# Future Improvements

- Hyperparameter tuning
- Deep Learning with LSTM
- BERT Transformer model
- Flask/FastAPI deployment
- Streamlit Web Application
- Real-time sentiment prediction

---

# Author

**Ritika Rani**

Machine Learning & Data Science Enthusiast

Completed as part of the **DecodeLabs Machine Learning Internship**.

---

# License

This project is intended for educational and learning purposes.
