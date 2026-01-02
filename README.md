## Titanic Survival Prediction (Random Forest)

This project implements a **machine learning pipeline** to predict passenger survival on the Titanic dataset using a **Random Forest classifier**.  
The focus is on **clean preprocessing, meaningful feature engineering, and model interpretability**.

---

### 📊 Dataset
- Titanic passenger dataset (`titanic_dataset.csv`)
- Target variable: **Survived**
- Features include demographic, ticket, and cabin-related information

---

### ⚙️ Methodology

**Data Preprocessing**
- Extracted passenger **titles** from names
- Handled missing values in *Age*, *Fare*, *Embarked*, and *Cabin*
- Reduced cabin information to first letter (or `U` for unknown)

**Feature Engineering**
- Created **FamilySize** from `SibSp` and `Parch`
- Grouped rare titles into a single category
- One-hot encoded categorical variables

**Model**
- Random Forest Classifier (`n_estimators = 100`)
- Train–test split: **80% / 20%**

---

### 📈 Results

- **Accuracy:** ~80.5%
- Strong balance between precision and recall
- Feature importance analysis highlights key predictors such as:
  - Passenger class
  - Sex
  - Age
  - Fare
  - Family size

---

### 🔍 Model Evaluation
- Accuracy score
- Confusion matrix
- Classification report (precision, recall, F1-score)
- Feature importance visualization for interpretability

---

### 🛠️ Tools & Libraries
Python · pandas · NumPy · scikit-learn · matplotlib · seaborn

---

### 🚀 Future Improvements
- Hyperparameter tuning
- Cross-validation
- Comparison with other classifiers (Logistic Regression, XGBoost)
- Probabilistic calibration and ROC analysis

---

*This project demonstrates an end-to-end supervised learning workflow with an emphasis on interpretability and feature-driven modeling.*

Gitty Up final test

