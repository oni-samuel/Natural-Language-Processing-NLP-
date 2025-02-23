# Natural Language Processing (NLP) Project

## 📌 Overview
This project demonstrates **Natural Language Processing (NLP)** techniques using data collected from an API request. The workflow includes:

- **Data Collection** from an external API
- **Exploratory Data Analysis (EDA)** to inspect textual features
- **Text Preprocessing** (cleaning and transformation)
- **Feature Extraction** using `CountVectorizer`

## 🛠️ Libraries Used
```python
import requests
import re
import nltk
import sklearn
import pandas as pd
```

---

## 🔍 Step 1: API Request & Data Extraction
We retrieve business data using the **RapidAPI Local Business Data API**. The response is stored as a JSON object and normalized into a Pandas DataFrame.



## 📊 Step 2: Exploratory Data Analysis (EDA)
We define a function `SEDA` (Simple EDA) to analyze the text column for patterns like URLs, email addresses, mentions, special characters, and emojis.


## 🧼 Step 3: Text Preprocessing
The `pre_processing` function cleans text by removing **HTML tags, URLs, mentions, emails, punctuation, digits, stopwords**, and applies **stemming or lemmatization**.



## 🔠 Step 4: Feature Extraction with `CountVectorizer`




## 📌 Summary
✅ Collected text data via API  
✅ Performed **Exploratory Data Analysis (EDA)**  
✅ Cleaned text by **removing HTML tags, URLs, mentions, emails, punctuation, digits, stopwords, emojis**  
✅ Applied **stemming and lemmatization**  
✅ Transformed text into a **Bag-of-Words model** using `CountVectorizer`  

This project provides a strong foundation for further **sentiment analysis, text classification, or NLP modeling**! 🚀


