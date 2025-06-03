
# Review Rating Prediction

## Project Overview

This project builds machine learning models to predict product or service ratings based on customer review text. Using Natural Language Processing (NLP) techniques and classification algorithms, the models aim to accurately classify the rating (1-5) from review content.

---

## Dataset

- The dataset contains customer reviews and their associated ratings.
- Reviews are processed using TF-IDF vectorization to transform text into numerical features.
- Ratings are the target labels for classification.

---

## Key Features

- **Text Vectorization:** Uses `TfidfVectorizer` to convert review text into TF-IDF features.
- **Data Preprocessing:** Splitting dataset into training and testing sets; features are standardized using `StandardScaler`.
- **Modeling:**
  - **K-Nearest Neighbors (KNN):** Hyperparameters optimized with Optuna for best accuracy.
  - **Logistic Regression:** Hyperparameters including penalty type, regularization strength, and solver tuned via Optuna.
- **Evaluation:** Model performance evaluated using classification reports including precision, recall, and F1-score.
- **Prediction Function:** Provides a reusable function to predict ratings from new review text input.

---


## Usage

1. **Data Preparation:** Load your review dataset with columns for text (`review_text`) and ratings (`rating`).
2. **Feature Extraction:** Vectorize reviews using TF-IDF.
3. **Split and Scale:** Split data into train/test sets and apply standard scaling.
4. **Hyperparameter Tuning:** Run Optuna to find the best model parameters for KNN and Logistic Regression.
5. **Model Training:** Train best models with optimized parameters.
6. **Evaluation:** Use classification reports to assess performance.
7. **Predict:** Use the `predict_rating` function to classify new reviews.

---

## Results Summary

- KNN achieved an accuracy of ~56% on training folds.
- Logistic Regression reached accuracy of ~67% in cross-validation.
- Model performance is affected by data imbalance and text complexity.
- Further improvements possible with larger datasets and more advanced NLP models.

---

## Future Work

- Explore deep learning models like LSTM or BERT for better text understanding.
- Address class imbalance with techniques such as SMOTE or class weighting.
- Implement ensemble models combining KNN and Logistic Regression.
- Expand dataset for improved generalization.

---

## Author

Oni Samuel Oluwapelumi  
Email: onis784@gmail.com  
GitHub: [https://github.com/oni-samuel](https://github.com/oni-samuel)  
LinkedIn: [https://www.linkedin.com/in/samuel-oni](https://www.linkedin.com/in/samuel-oni)
