# Student Pass/Fail Prediction using Binary Logistic Regression

## Activity 2 – Regression and Classification Algorithms (CIE 2)
Submission GitHub ID: https://github.com/complexiota.
PROJECT LINK - https://github.com/gg-nishka/RCA-Activity-2-AD-3342-
## 1. Project Overview
This project uses **Binary Logistic Regression** to predict whether a student will pass or fail based on study hours and attendance. The goal is to classify a student into one of two categories (Pass or Fail).

## 2. Problem Statement
Predict a student's result using:
- **Study Hours** – number of hours spent studying
- **Attendance** – attendance percentage

**Target:** Pass/Fail (binary classification)

- `1` = Pass
- `0` = Fail

## 3. Dataset
A small synthetic dataset was created for this activity with 60 student records.

| Column | Description | Type |
|---|---|---|
| `Study_Hours` | Daily study hours | Numerical input feature |
| `Attendance` | Attendance percentage | Numerical input feature |
| `Pass_Fail` | Pass (1) or Fail (0) | Binary target |

The dataset is provided in `student_pass_fail_dataset.csv` in this repository. Since it is synthetic, it is intended for learning and demonstration only—not for real student evaluation.

## 4. Tools and Libraries
- Python
- Google Colab / Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Scikit-learn

## 5. Activity Steps
1. Load the dataset and inspect sample rows and data information.
2. Check for missing values and explore class distribution.
3. Plot relationships between Study Hours, Attendance, and Pass/Fail.
4. Separate input features and target; split the data into training and testing sets using stratification.
5. Train a Binary Logistic Regression model.
6. Predict class probabilities and apply a 0.5 threshold to obtain Pass/Fail labels.
7. Compare thresholds 0.3, 0.5, and 0.7 using Accuracy, Precision, Recall, and F1-score.
8. Evaluate the model using the confusion matrix, Accuracy, Precision, Recall, Specificity, F1-score, and ROC-AUC.
9. Plot the ROC curve and compare the model with a simple baseline.
10. Predict the result for a new student example.

## 6. Logistic Regression
Logistic Regression estimates the probability that a student will pass.

The probability is converted into a class using a threshold:

- Probability >= 0.5 → Pass (`1`)
- Probability < 0.5 → Fail (`0`)

The threshold can be changed to 0.3 or 0.7 to see how the classification results change.

## 7. Evaluation Metrics
- **Accuracy:** Overall proportion of correct predictions.
- **Precision:** Among predicted passes, how many are actually passes.
- **Recall:** Among actual passes, how many are correctly predicted as passes.
- **Specificity:** Among actual fails, how many are correctly predicted as fails.
- **F1-score:** Combines Precision and Recall into one score.
- **ROC-AUC:** Measures how well the model distinguishes between Pass and Fail.

## 8. Conclusion
This activity demonstrates how Binary Logistic Regression can classify students as Pass or Fail using study hours and attendance. The model is evaluated with multiple classification metrics, different thresholds, and a ROC curve. The results are based on a synthetic dataset and should not be used to make real academic decisions.

## 9. Repository Files
- `student_pass_fail_dataset.csv` – dataset used for the activity
- `README.md` – project description and activity summary
- Notebook – code, plots, threshold comparison, model evaluation, and prediction (upload the notebook to this repository)

## How to Run
1. Open the notebook in Google Colab.
2. Upload `student_pass_fail_dataset.csv` when prompted or place it in the Colab working directory.
3. Run the notebook cells from top to bottom.
