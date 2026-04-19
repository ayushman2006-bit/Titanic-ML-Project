# Titanic Survival Prediction 

A machine learning project that predicts passenger survival on the Titanic using multiple models, with a focus on feature engineering, model comparison, and evaluation using real-world metrics.

Goal: Identify the most reliable model and understand key factors influencing survival.

## Dataset
- Source: Kaggle Titanic Dataset
- Features include: age, sex, passenger class, fare, family relations, etc.
- Target variable: `survived` (0 = No, 1 = Yes)

## Workflow
1. Data Cleaning
   - Removed redundant column (`alive`) to prevent data leakage
   - Handled missing values (mean for age, mode for embarked)

2. Feature Engineering
   - Created `family_size`
   - Created `is_alone` feature

3. Data Preprocessing
   - One-hot encoding for categorical variables
   - Feature-target split

4. Model Training
   - Logistic Regression (baseline model)
   - Random Forest (ensemble model)

5. Model Evaluation
   - Compared models using multiple performance metrics

## Models Used
- Logistic Regression
- Random Forest Classifier

## Results & Model Comparison

| Model                | Accuracy | F1 Score | ROC-AUC |
|---------------------|----------|----------|--------|
| Logistic Regression | ~80%     | ~0.78    | ~0.84  |
| Random Forest       | ~83%     | ~0.81    | ~0.87  |
  Best Model: Random Forest (based on ROC-AUC)

## Evaluation Metrics
- Confusion Matrix
- Classification Report (Precision, Recall, F1-score)
- ROC Curve
- 
## Visualizations
- Confusion Matrix
- ROC Curve
- Feature Importance Plot
- Survival Count Plot
- 
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

## Why This Project Matters
This project demonstrates real-world machine learning workflow:
- Identifying and fixing data leakage
- Building meaningful features
- Comparing models using multiple evaluation metrics
- Interpreting model behavior instead of just reporting accuracy

##  What I Learned
- Importance of avoiding data leakage
- Proper handling of categorical variables
- Feature engineering improves model performance
- Model comparison is important

---

If you like this project, consider giving it a star!
