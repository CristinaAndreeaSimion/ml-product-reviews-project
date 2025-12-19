# ml-product-reviews-project
A complete project for classifying product review sentiment
# 💖 Sentiment Analysis ML Project (Complete Pipeline)

## 1. Project Overview

This repository contains a complete machine learning pipeline for **sentiment analysis** of product reviews using Python and scikit-learn.

The project was developed as part of a learning module, where we demonstrated all typical phases of a machine learning workflow — from raw data to a ready-to-use trained model.

---

## 2. Project Structure

├── data/
│   └── product_reviews_full.csv  # dataset
│
├── notebooks/
│   └── exploratory_analysis.ipynb  # EDA and preprocessing
│
├── src/
│   ├── train_model.py  # Script for training and saving the model
│   └── test_model.py   # Script for testing saved model
│
└── README.md

---

## 3. Data Cleaning & Preprocessing
- Removed missing values
- Standardized sentiment labels (positive / negative / neutral)
- Parsed and validated price
- Converted review text to numerical length

---

## 4. Feature Engineering
- Selected meaningful input features: `review_title`, `review_text`, and `review_length`
- Removed irrelevant columns
- Explored correlation between price and sentiment

---

## 5. Model Training & Evaluation
- Compared multiple ML models (Logistic Regression, Naive Bayes, Decision Tree, Random Forest, SVM)
- Used `ColumnTransformer` and `Pipeline` for unified preprocessing
- Evaluated using precision, recall, F1-score, and confusion matrix

---

## 6. Final Model Training
- Trained final model on full dataset
- Saved the pipeline using `joblib` to `sentiment_model.pkl`

---

## 7. Inference & Usage
- Loaded saved model
- Built an interactive interface for predicting sentiment of new reviews
- Enabled real-time testing via console input

---

## 🚀 How to Use

### 🏋️ Train the Model
```bash
cd src
python train_model.py

This will create a file called sentiment_model.pkl in the root directory.

🔍 Run Inference

Use the interactive script (model_test.py) to classify new reviews using the trained model.

👨‍💻 Author

This repository was developed as part of an educational program on practical machine learning using Python.
All steps were carefully documented and modularized to help students understand and reproduce the entire workflow.

📄 License

This project is open-source and freely available for educational use.
