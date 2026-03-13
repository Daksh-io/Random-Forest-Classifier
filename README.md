# 🌲 Random Forest Sentiment Analysis

A Machine Learning project that performs **multi-class sentiment classification** on text data using **TF-IDF vectorization and a Random Forest classifier**.

The project demonstrates a complete **ML pipeline for Natural Language Processing (NLP)** including data preprocessing, feature engineering, model training, and model interpretation.

---

# 📌 Project Overview

This project builds a sentiment classification model that predicts the sentiment of a given text using a **Random Forest algorithm**.

The workflow includes:

- Data loading and preprocessing
- Text feature extraction using TF-IDF
- Training a Random Forest model
- Hyperparameter tuning using GridSearchCV
- Model evaluation
- Feature importance analysis

---

# 🧠 Machine Learning Pipeline

The model is implemented using **Scikit-learn Pipeline**, combining:

TF-IDF Vectorizer → Random Forest Classifier

This approach ensures that text preprocessing and model training happen in a single pipeline.

---

# ⚙️ Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Jupyter Notebook / Google Colab

---

# 📂 Dataset

The dataset contains text samples labeled with their corresponding sentiment classes.

Example structure:

| Text | Sentiment |
|-----|-----|
| I love this product | Positive |
| This is terrible | Negative |
| It is okay | Neutral |

The dataset is cleaned by removing rows with missing text or sentiment labels.

---

# 🔎 Feature Engineering

Text data is converted into numerical features using:

**TF-IDF (Term Frequency – Inverse Document Frequency)**

This method captures the importance of words across the dataset while reducing the influence of common words.

---

# 🌲 Model: Random Forest Classifier

Random Forest is an ensemble learning method that builds multiple decision trees and combines their predictions.

Advantages:

- Handles high-dimensional data
- Reduces overfitting
- Works well for text classification tasks

---

# 🔧 Hyperparameter Tuning

Model parameters are optimized using **GridSearchCV** with **Stratified K-Fold cross-validation**.

Parameters tuned include:

- `n_estimators`
- `max_depth`
- `min_samples_split`
- `min_samples_leaf`

This ensures the model finds the best configuration for the dataset.

---

# 📊 Model Evaluation

Model performance is evaluated using:

- **Classification Report**
- Precision
- Recall
- F1 Score

These metrics help measure how well the model predicts sentiment classes.

---

# 📈 Feature Importance Analysis

The project also analyzes **which words influence predictions the most**.

Steps:

1. Extract feature names from TF-IDF
2. Get importance scores from Random Forest
3. Rank features by importance
4. Visualize the top contributing words

This helps understand **what words the model relies on for prediction**.

---

# 🚀 How to Run the Project

### 1 Clone the repository

```bash
git clone https://github.com/yourusername/random-forest-sentiment-analysis.git
