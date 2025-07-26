# Titanic - Machine Learning from Disaster 🛳️

This project is a Kaggle competition solution designed for educational purposes. It focuses on applying supervised machine learning techniques to predict passenger survival on the Titanic.

---

## 📁 Project Structure

- `train.csv` & `test.csv`: Source datasets used for training and evaluation.
- `v1.ipynb`: Main notebook with all preprocessing, modeling, and prediction code.
- `v1_explanations.ipynb`: Annotated version with detailed markdown explanations.
- `submission.csv`: Final prediction file for Kaggle submission.
- `Titanic Survival Prediction.pptx`: Presentation summarizing the project workflow and results.

---

## 🔍 Summary of Steps

### 📥 Data Loading & Initial Analysis
- Loaded and explored both `train.csv` and `test.csv`.
- Identified and visualized missing values.

### 🔄 Data Preprocessing
- Combined train and test sets for consistent processing.
- Encoded categorical variables (`Sex`, `Embarked`) using LabelEncoder.
- Imputed missing `Age` values using `KNNImputer`.
- Split combined data back into train/test sets.

### 🧹 Feature Engineering
- Dropped low-informative features (`Cabin`, `Name`, `Ticket`).
- Handled missing values in `Embarked` and `Fare`.
- Created new features: `FamilySize` and `IsAlone`.

### 🤖 Modeling & Evaluation
- Trained and compared multiple models:
  - Logistic Regression
  - K-Nearest Neighbors (KNN)
  - Support Vector Machine (SVM)
  - Random Forest
  - XGBoost (tuned via GridSearchCV)
- **Best model: Tuned XGBoost with 85.36% accuracy**

### 📊 Prediction & Submission
- Generated predictions on test set.
- Created `submission.csv` with `PassengerId` and predicted `Survived` column.

### 📽️ Presentation Slides
- Embedded in the notebook as markdown:
  - Title
  - Dataset Overview
  - Preprocessing Steps
  - Model Comparison
  - Key Findings
  - Final Results & Recommendations

---

## 📌 Notes

- This project is part of a machine learning learning path using real-world Kaggle challenges.
- Focus was on practical application, explainability, and modular workflow.

---
