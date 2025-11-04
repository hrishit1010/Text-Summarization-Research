# Text-Summarization-Research
# Machine Learning Model Analysis

This repository contains Jupyter Notebooks for two separate machine learning projects:
1.  A classification project to predict user purchases from the "Social Network Ads" dataset.
2.  An NLP project to classify restaurant reviews as positive or negative.

---

## Project 1: Social Network Ads Prediction

This project compares four different classification models to predict whether a user will purchase a product based on their age, estimated salary, and gender.

**Dataset:** `Social_Network_Ads.csv`
**Common Preprocessing:** Features are scaled using `StandardScaler`.

### Model Performance Summary

| Notebook | Model | Test Accuracy |
| :--- | :--- | :---: |
| `SVM_Project.ipynb` | **Support Vector Machine (RBF Kernel)** | **93.00%** |
| `XGBoost.ipynb` | **XGBoost Classifier** | **92.00%** |
| `RandomForest_Bagging.ipynb` | **Random Forest Classifier** (10 trees) | **91.00%** |
| `Logistic_Regression.ipynb` | **Logistic Regression** | **89.00%** |

---

## Project 2: Restaurant Review NLP

This project uses Natural Language Processing (Bag of Words) and ensemble methods to classify restaurant reviews as positive (1) or negative (0).

**Dataset:** `Restaurant_Reviews.tsv`
**Preprocessing:** `CountVectorizer` (Bag of Words model), NLTK stopwords removal.

### Model Performance (`RandomForest_Bagging (1).ipynb`)

* **Model 1: Random Forest Classifier**
    * Parameters: `n_estimators=500`, `criterion='entropy'`
    * **Accuracy:** **72.00%**

* **Model 2: Bagging Classifier**
    * Base Model: Random Forest
    * Parameters: `n_estimators=500`
    * **Accuracy:** **72.50%**
