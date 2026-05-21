# Fake News Detection Using Machine Learning

## Project Overview

This project is a **Fake News Detection System** developed using Python and Machine Learning.  
The model analyzes news statements and predicts whether the news is:

- Fake News
- Real News

The project uses Natural Language Processing (NLP) techniques and a machine learning classifier to classify news statements based on textual patterns.

---

# Features

- Text preprocessing using NLP
- Stopword removal
- Lemmatization
- TF-IDF vectorization
- Fake news classification
- Data visualization
- Confusion matrix visualization
- Model saving using Pickle
- Real-time news prediction

---

# Technologies Used

## Programming Language
- Python

## Libraries Used

- pandas
- numpy
- seaborn
- matplotlib
- nltk
- scikit-learn
- pickle
- regex

---

# Machine Learning Algorithm

This project uses:

:contentReference[oaicite:0]{index=0}

for fake news classification.

---

# Natural Language Processing Techniques

The following NLP techniques are used:

- Tokenization
- Stopword Removal
- Lemmatization
- TF-IDF Vectorization

---

# Project Structure

```bash
Fake-News-Detection/
│
├── train.tsv
├── fake_news_detection.py
├── model.pkl
├── README.md
└── requirements.txt
```

---

# Dataset Information

The dataset contains multiple columns related to political statements.

| Column Name | Description |
|-------------|-------------|
| Label | Truthfulness label |
| Statement | News statement |
| Subject | Subject category |
| Speaker | Speaker name |
| Party | Political party |
| Context | Context of statement |

---

# Labels in Dataset

The dataset contains the following labels:

- true
- mostly-true
- half-true
- barely-true
- false
- pants-fire

These labels are later categorized into:
- Real News
- Fake News

---

# Installation Guide

## Step 1: Clone the Repository

```bash
git clone https://github.com/your-username/fake-news-detection.git
```

---

## Step 2: Navigate to Project Folder

```bash
cd fake-news-detection
```

---

## Step 3: Install Required Libraries

```bash
pip install -r requirements.txt
```

---

# Requirements File

Create a file named `requirements.txt` and add:

```txt
pandas
numpy
matplotlib
seaborn
nltk
scikit-learn
```

---

# Download NLTK Resources

The project automatically downloads:

- stopwords
- punkt
- wordnet

using:

```python
nltk.download('stopwords')
nltk.download('punkt')
nltk.download('wordnet')
```

---

# Workflow of the Project

## 1. Load Dataset

The dataset is loaded using:

```python
pd.read_csv()
```

---

## 2. Data Cleaning

The following preprocessing steps are performed:

- Remove special characters
- Convert text to lowercase
- Remove stopwords
- Lemmatization

Example:

```python
review = re.sub(r'[^a-zA-Z\s]', '', review)
review = review.lower()
```

---

# Text Preprocessing

The project uses:

:contentReference[oaicite:1]{index=1}

to convert textual data into numerical vectors.

Formula:

:contentReference[oaicite:2]{index=2}

---

# Train-Test Split

The dataset is divided into:
- 70% Training Data
- 30% Testing Data

Using:

```python
train_test_split()
```

---

# Model Training

The model is trained using:

```python
classifier.fit(tfidf_X_train, Y_train)
```

---

# Prediction

The model predicts whether news is:
- Fake
- Real

Example:

```python
prediction = loaded_model.predict(vectorized_input_data)
```

---

# Accuracy Evaluation

The model performance is evaluated using:

- Accuracy Score
- Confusion Matrix

Formula for Accuracy:

:contentReference[oaicite:3]{index=3}

---

# Confusion Matrix

The confusion matrix helps visualize:
- Correct predictions
- Incorrect predictions

Generated using:

```python
confusion_matrix()
```

---

# Model Saving

The trained model is saved using Pickle.

```python
pickle.dump(classifier, open('model.pkl', 'wb'))
```

---

# Real-Time News Detection

The function:

```python
fake_news_det(news)
```

allows users to input custom news statements for prediction.

---

# Example Predictions

## Fake News Example

```text
Donald Trump said that global warming is a hoax invented by China.
```

Output:

```text
Prediction of the News : Looking Fake News
```

---

## Real News Example

```text
President Biden signed the Infrastructure Investment and Jobs Act into law.
```

Output:

```text
Prediction of the News : Looking Real News
```

---

# Output Visualizations

The project generates:
- Distribution Plot
- Confusion Matrix

---

# Sample Output

```bash
Accuracy: 92.45%
```

---

# Future Improvements

Possible enhancements:
- Add Deep Learning models
- Use LSTM or BERT models
- Create a Web Application
- Add live news API integration
- Improve prediction accuracy

---

# Learning Outcomes

By completing this project, you will learn:
- Natural Language Processing (NLP)
- Text preprocessing
- TF-IDF Vectorization
- Machine Learning Classification
- Model Evaluation
- Confusion Matrix Analysis

---

# GitHub Topics

Add these topics to your repository:

- python
- machine-learning
- fake-news-detection
- nlp
- text-classification
- scikit-learn
- tfidf
- passive-aggressive-classifier
- data-science

---

# Author

**Vinesh R**

---

# License

This project is open-source and available under the MIT License.# fake_news_detection_master-
