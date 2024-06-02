# Titanic Survival Prediction

## Project Overview
The objective of this project is to predict the survival of passengers on the Titanic using machine learning techniques. The dataset is provided by Kaggle and contains various features about the passengers.

## Data Exploration
Exploration of the dataset revealed the following insights:
- The survival rate was about 38%.
- Females had a higher survival rate than males.
- Passengers in higher classes (1st class) had a higher survival rate.

## Data Cleaning and Preprocessing
- Missing values in the 'Age' column were filled with the median.
- Missing values in the 'Embarked' column were filled with the mode.
- Categorical variables were one-hot encoded.
- Unnecessary columns such as 'Name', 'Ticket', and 'Cabin' were dropped.

## Model Selection and Training
- Tried Logistic Regression, Decision Tree, Random Forest, and Gradient Boosting.
- Performed hyperparameter tuning using Grid Search.
- Best model: Random Forest with parameters:
  - `max_depth`: 10
  - `min_samples_leaf`: 2
  - `min_samples_split`: 10
  - `n_estimators`: 100

## Model Evaluation
- Best cross-validation score: 82.86%
- Confusion Matrix and Classification Report for the final model:
  - Accuracy: 91.06%
  - Precision, Recall, F1-Score for each class:
    - Not Survived: 0.90, 0.95, 0.93
    - Survived: 0.93, 0.85, 0.89

## Conclusion
The Random Forest model performed very well, achieving an accuracy of approximately 91%. The precision and recall for both classes indicate that the model is well-balanced and can correctly identify the majority of the cases. Future improvements could include more advanced feature engineering and exploring other sophisticated models.

## How to Use
1. Clone the repository: `git clone https://github.com/EhsaasSam/titanic-survival-prediction.git`
2. Navigate to the project directory: `cd titanic-survival-prediction`
3. Open the Jupyter Notebook: `jupyter notebook Titanic_Survival_Prediction.ipynb`
4. Run the cells in the notebook to reproduce the results.

## Repository
- [GitHub Repository](https://github.com/EhsaasSam/titanic-survival-prediction)
