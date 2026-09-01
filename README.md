# ML Student Performance Prediction and Model Evaluation

## 📌 Project Overview
This repository contains a complete machine learning workflow to analyze student habits and predict academic performance. The project applies Exploratory Data Analysis (EDA) and predictive modeling to understand how lifestyle factors (such as study hours, screen time, and mental health) impact student exam scores. 

The analysis is divided into two main machine learning tasks:
1. **Regression Task:** Predicting the exact exam score using a **Linear Regression** model.
2. **Classification Task:** Predicting whether a student will Pass or Fail (using a 50-mark threshold) with a **Logistic Regression** model.

## 📊 Dataset
The dataset used in this project is `Day18_19_student_habits_performance.csv`. It contains 1,000 records of students with the following key features:
* **Numerical Features:** Age, study hours per day, social media hours, Netflix hours, attendance percentage, sleep hours, exercise frequency, and mental health rating.
* **Categorical Features:** Gender, part-time job status, diet quality, internet quality, extracurricular participation, and parental education level.
* **Target Variable:** `exam_score` (Continuous for Regression, Binarized to Pass/Fail for Classification).

## 🚀 Project Workflow
1. **Exploratory Data Analysis (EDA):** 
   * Analyzed feature distributions and checked for outliers.
   * Investigated relationships and correlations between student habits and exam scores.
2. **Data Preprocessing:**
   * Handled missing values (imputed missing categorical data using mode).
   * Applied One-Hot Encoding for categorical variables.
   * Defined features (`X`) and target variables (`y`).
3. **Linear Regression (Score Prediction):**
   * Split data into 80% training and 20% testing sets.
   * Trained the model and evaluated using MAE, MSE, RMSE, and R² scores.
4. **Logistic Regression (Pass/Fail Classification):**
   * Transformed the target variable into a binary Pass (>=50) and Fail (<50) class.
   * Trained the model and evaluated using Accuracy, Precision, Recall, F1-Score, and a Confusion Matrix.
5. **Model Evaluation:**
   * Compared Train vs. Test metrics to confirm models were well-generalized with low bias and low variance.

## 💡 Key Insights Discovered
1. **Study time is the biggest lever:** `study_hours_per_day` shows the strongest positive relationship with exam scores.
2. **Attendance matters almost as much as study hours:** Simply showing up to class regularly is a meaningful predictor of academic success.
3. **Screen-time habits are linked to lower scores:** Both social media and Netflix hours show a clear negative relationship with exam scores.
4. **Mental health is an underrated academic factor:** A positive association exists between mental health ratings and exam performance.
5. **Simple models perform exceptionally well:** Basic linear and logistic regression models achieved strong, well-generalized performance, suggesting that exam performance is driven by clear behavioral factors rather than complex hidden interactions.

## 🛠️ Requirements & Libraries
To run this notebook, you will need the following Python libraries installed:
* `pandas`
* `numpy`
* `matplotlib`
* `seaborn`
* `scikit-learn`

## 🏃 How to Run
1. Clone this repository:
   ```bash
   git clone [https://github.com/abino-w/ML-Student-Performance-Prediction-and-Model-Evaluation-.git](https://github.com/abino-w/ML-Student-Performance-Prediction-and-Model-Evaluation-.git)
