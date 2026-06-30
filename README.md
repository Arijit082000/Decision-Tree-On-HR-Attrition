#  Employee Attrition Prediction using Decision Tree

##  Project Overview
This project builds a **Decision Tree Classifier** to predict whether an employee is likely to leave a company (Attrition). It includes data exploration, preprocessing, model training, and evaluation using the IBM HR Analytics dataset from OpenML.

##  Objective
- Predict employee attrition.
- Understand the impact of HR-related features.
- Compare a standard Decision Tree with a class-balanced Decision Tree.

##  Dataset
- **Source:** IBM HR Analytics Dataset (OpenML, Data ID: 43696)
- **Rows:** 1,470
- **Columns:** 35
- **Target Variable:** `Attrition`
  - Stayed
  - Left

##  Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

##  Exploratory Data Analysis
- Dataset overview
- Dataset information
- Missing value inspection
- Feature exploration

##  Data Preprocessing
- Encode categorical variables
- Train-test split
- Handle class imbalance using `class_weight='balanced'`

##  Machine Learning Model
**Algorithm:** Decision Tree Classifier

Parameters used:
- `max_depth=5`
- `random_state=42`

Balanced model:
- `class_weight='balanced'`

##  Model Performance

### Default Decision Tree
- **Accuracy:** 82.31%

### Balanced Decision Tree
- Improved recall for employees who left the company.
- Better handling of the imbalanced dataset.

##  Project Structure
```
Decision Tree on HR dataset.ipynb
README.md
```

##  Installation

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

Run the notebook:

```bash
jupyter notebook
```

##  Results
The standard Decision Tree achieved **82.31% accuracy**. Applying `class_weight='balanced'` improved the model's ability to identify employees who left, making it more suitable for an imbalanced HR dataset.

##  Future Improvements
- Hyperparameter tuning using GridSearchCV
- Random Forest and XGBoost comparison
- Feature importance analysis
- Cross-validation
- SHAP model explainability

##  Author
**Arijit Dasgupta**

