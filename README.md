# Natural Language Processing (NLP) & Machine Learning Project

## 📌 Overview
This project demonstrates Natural Language Processing (NLP) techniques and machine learning algorithms to analyze text data collected from an API request. The workflow includes:

- Data Collection from an external API
- Exploratory Data Analysis (EDA) to inspect textual features
- Text Preprocessing (cleaning and transformation)
- Feature Extraction using TF-IDF
- Machine Learning Model Implementation (KNN, Logistic Regression, Decision Tree)
- Hyperparameter Tuning and Model Evaluation
- Deployment using Streamlit

## 🎯 Business Problem
Businesses need to analyze customer reviews and location data to improve services and attract more customers. Manually processing this data is inefficient, making it difficult to identify key factors influencing business success. A machine learning model can help predict business performance based on reviews and location insights, enabling data-driven decision-making.

## 🛠️ Libraries Used
```python
import requests
import re
import nltk
import sklearn
import pandas as pd
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt
from sklearn.feature_extraction.text import TfidfVectorizer
from sklearn.model_selection import train_test_split
from sklearn.neighbors import KNeighborsClassifier
from sklearn.linear_model import LogisticRegression
from sklearn.tree import DecisionTreeClassifier
from sklearn.metrics import accuracy_score, classification_report
```

## 🔍 Step 1: API Request & Data Extraction
We retrieve business data using the RapidAPI Local Business Data API. The response is stored as a JSON object and normalized into a Pandas DataFrame.

## 📊 Step 2: Exploratory Data Analysis (EDA)
We define a function `SEDA` (Simple EDA) to analyze the text column for patterns like URLs, email addresses, mentions, special characters, and emojis.

## 🧼 Step 3: Text Preprocessing
The `pre_processing` function cleans text by:
- Removing HTML tags, URLs, mentions, emails, punctuation, digits, and emojis
- Converting text to lowercase
- Removing stopwords
- Applying stemming or lemmatization

## 🔠 Step 4: Feature Extraction with TF-IDF
To transform text into numerical features, we use TF-IDF (Term Frequency-Inverse Document Frequency) representation.

## 🏆 Step 5: Machine Learning Model Implementation
### K-Nearest Neighbors (KNN)



## 🔄 Step 6: Hyperparameter Tuning & Model Evaluation
We fine-tune the models using GridSearchCV or RandomizedSearchCV to achieve optimal performance.
`



## 📌 Summary
✅ Collected text data via API
✅ Performed Exploratory Data Analysis (EDA)
✅ Cleaned text by removing HTML tags, URLs, mentions, emails, punctuation, digits, stopwords, and emojis
✅ Applied stemming and lemmatization
✅ Transformed text into numerical features using TF-IDF
✅ Implemented Machine Learning models (KNN, Logistic Regression, Decision Tree)
✅ Fine-tuned models for improved performance
✅ Deployed the best model using Streamlit

This project helps strengthen essential data science skills, including data preprocessing, model evaluation, hyperparameter tuning, and deployment techniques.
