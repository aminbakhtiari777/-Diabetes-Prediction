# Diabetes Prediction

This project predicts whether a person has diabetes using the Pima Indians Diabetes Dataset.

## Project Steps

- Loaded the dataset
- Checked missing values
- Detected suspicious zero values
- Replaced invalid zero values with median values
- Analyzed feature correlation with the target
- Trained a Logistic Regression model
- Trained a Random Forest model
- Compared accuracy, recall, precision, and F1-score
- Extracted feature importance from Random Forest

## Dataset

The dataset contains 768 rows and 9 columns.

Target column:

- `Outcome`
  - 0 = No diabetes
  - 1 = Diabetes

Main features:

- Glucose
- BMI
- Age
- Pregnancies
- Insulin
- BloodPressure
- SkinThickness
- DiabetesPedigreeFunction

## Models

### Logistic Regression

Accuracy: 75.3%

Recall for diabetes class: 62%

### Random Forest

Accuracy: 74.7%

Recall for diabetes class: 67%

## Conclusion

Although Logistic Regression had slightly higher accuracy, Random Forest performed better in detecting diabetic patients because it had higher recall for class 1.

In medical prediction tasks, recall is very important because missing a real patient can be more dangerous than giving a false alarm.

## Most Important Features

According to Random Forest feature importance:

1. Glucose
2. BMI
3. Age
4. DiabetesPedigreeFunction
5. Insulin

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
