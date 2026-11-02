# Project Report: Student Pass Prediction Using Logistic Regression

## 1. Abstract
This project demonstrates binary classification using Logistic Regression. It estimates the probability of a student passing an exam based on study hours and classifies the result as likely to pass or not pass. Python and Scikit-learn are used for training, evaluation, prediction, and visualization.

## 2. Problem Statement
Build a simple classification model that predicts a binary exam outcome from the number of hours a student studies.

## 3. Objectives
- Understand Logistic Regression.
- Prepare a binary-labelled dataset.
- Train and test a classification model.
- Predict the probability of passing for a new study-hour value.
- Evaluate performance using classification metrics.
- Plot the observations and predicted probability curve.

## 4. Tools and Technologies
- Python
- Pandas and NumPy
- Matplotlib
- Scikit-learn
- VS Code, Jupyter Notebook, or Google Colab

## 5. Theory
Despite its name, Logistic Regression is commonly used for classification. It first calculates a linear score, then maps it to a probability with the sigmoid function:

`p = 1 / (1 + e^-(b0 + b1x))`

Here, `x` is study hours, `b0` is the intercept, `b1` is the coefficient, and `p` is the estimated probability of class 1. With a threshold of 0.5, probability values at least 0.5 are classified as `1`; lower values are classified as `0`.

## 6. Dataset
The included artificial dataset contains:
- `StudyHours`: number of hours studied
- `Passed`: target label, where `0` means Not Passed and `1` means Passed

The data is constructed only for demonstration and does not represent real students.

## 7. Methodology
1. Import required libraries.
2. Load the sample dataset.
3. Separate the input feature (`StudyHours`) and target (`Passed`).
4. Split data into training and testing subsets.
5. Scale the input feature and train Logistic Regression.
6. Predict classes and probabilities on test data.
7. Calculate accuracy, precision, recall, F1-score, and confusion matrix.
8. Ask for a new study-hours value and predict its class/probability.
9. Plot sample outcomes and the fitted probability curve.

## 8. Evaluation Metrics
- **Accuracy:** fraction of test predictions that are correct.
- **Precision:** fraction of predicted passes that are actually passes.
- **Recall:** fraction of actual passes identified by the model.
- **F1-score:** harmonic mean of precision and recall.
- **Confusion matrix:** counts correct and incorrect predictions for each class.

Metrics depend on the train/test split and the small artificial dataset; they are not evidence of real-world predictive ability.

## 9. Expected Output
The program displays evaluation metrics, a confusion matrix, test predictions with estimated probabilities, and a plot. It then asks for study hours and prints the estimated probability of passing and the predicted class.

## 10. Limitations
- The dataset is small and artificial.
- One feature is not enough to assess academic performance reliably.
- Results can vary with the split and dataset.
- The model should not be used for real student evaluation.

## 11. Future Scope
Use a larger, ethically collected dataset with appropriate consent and relevant features; compare Logistic Regression with other classification models; and build a simple web interface for demonstration.

## 12. Conclusion
This project demonstrates a basic supervised learning workflow for binary classification, including preprocessing, model training, probability prediction, evaluation, and visualization.
