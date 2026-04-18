# Titanic Survival Prediction 🚢

## Project Overview
Machine Learning project predicting Titanic survival using Logistic Regression and Random Forest with feature engineering.

## Dataset
- Titanic dataset (cleaned version)
- Contains passenger details like age, class, gender, etc.

## Steps Performed
- Data Cleaning (handling missing values)
- Feature Engineering (family size, is_alone)
- Encoding categorical variables
- Train-test split
- Model training and comparison

## Models Used
- Logistic Regression
- Random Forest Classifier

## Results
- Accuracy: ~81–83%
- Balanced performance across classes

## Evaluation Metrics
- Confusion Matrix
- Classification Report (Precision, Recall, F1-score)
- ROC Curve

## Key Insights
- Gender and passenger class are strong predictors
- Family size impacts survival probability

## Future Improvements
- Hyperparameter tuning (GridSearchCV)
- Try advanced models (XGBoost)
- Deploy as a web app

## Tools & Libraries
- Python
- Pandas, NumPy
- Seaborn, Matplotlib
- Scikit-learn

## Challenges Faced
- Data leakage due to 'alive' column → removed it
- Encoding issues (string to float) → solved using pd.get_dummies
- Got 100% accuracy due to leakage → fixed preprocessing
- Handled missing values in 'age' and 'embarked'
- Faced KeyError due to dataset mismatch → fixed by checking columns
- Learned importance of proper train-test split

##  What I Learned
- Importance of avoiding data leakage
- Proper handling of categorical variables
- Feature engineering improves model performance
- Model comparison is important

---

If you like this project, consider giving it a star!
