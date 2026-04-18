Titanic Survival Prediction

Project Overview:
Machine Learning project predicting Titanic survival using Logistic Regression and Random Forest with feature engineering.

Dataset:
-> Titanic dataset (cleaned version)
-> Contains passenger details like age, class, gender, etc.

Steps Performed:
-> Data Cleaning (handling missing values)
-> Feature Engineering (family size, is_alone)
-> Encoding categorical variables
-> Train-test split
-> Model training and comparison

Models Used:
-> Logistic Regression
-> Random Forest Classifier

Results:
-> Accuracy: ~81–83%
-> Balanced performance across classes

Evaluation Metrics:
-> Confusion Matrix
-> Classification Report (Precision, Recall, F1-score)
-> ROC Curve

Key Insights:
->Gender and passenger class are strong predictors
->Family size impacts survival probability

Future Improvements:
-> Hyperparameter tuning (GridSearchCV)
-> Try advanced models (XGBoost)
-> Deploy as a web app

Tools & Libraries:
-> Python
-> Pandas, NumPy
-> Seaborn, Matplotlib
-> Scikit-learn
Challenges Faced:

-> Faced data leakage issue due to presence of 'alive' column, which directly indicated survival outcome. Fixed by removing the column.
-> Encountered errors with categorical data encoding (string to float conversion). Solved using one-hot encoding (pd.get_dummies).
-> Got unrealistic 100% accuracy initially due to improper preprocessing and leakage.
-> Handled missing values in 'age' and 'embarked' columns using mean and mode.
-> Faced KeyError due to dataset mismatch and resolved by checking column names before operations.
-> Learned importance of proper train-test split to avoid overfitting.

If you like this project, consider giving it a star!
