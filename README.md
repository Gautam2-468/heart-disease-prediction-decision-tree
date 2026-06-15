# ❤️ Heart Disease Prediction using Decision Tree Classifier

## 📌 Project Overview

This project uses a Decision Tree Classifier to predict whether a patient is likely to have heart disease based on various medical attributes. The project covers the complete machine learning workflow, including data cleaning, exploratory data analysis (EDA), visualization, model building, overfitting detection, hyperparameter tuning, and performance evaluation.

---

##  Objective

The goal of this project is to build a machine learning model that can classify patients into:

* 0 → No Heart Disease
* 1 → Heart Disease

using patient health-related features.

---

##  Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn

---

##  Exploratory Data Analysis (EDA)

The following steps were performed:

* Dataset inspection using `.head()`, `.info()`, and `.shape()`
* Missing value analysis
* Duplicate value removal
* Correlation analysis
* Correlation Heatmap
* Target Variable Distribution
* Feature Importance Visualization

---

##  Model Building

### Decision Tree Classifier

The dataset was split into training and testing sets using Train-Test Split.

A Decision Tree Classifier was trained using:

```python
DecisionTreeClassifier(max_depth=3, random_state=42)
```

The `max_depth` parameter was used to reduce overfitting and improve model generalization.

---

##  Model Performance

### Training Accuracy

```text
84.64%
```

### Testing Accuracy

```text
75.41%
```

### Classification Report

```text
Precision : 0.74
Recall    : 0.74
F1 Score  : 0.74
Accuracy  : 0.74
```

---

##  Feature Importance

The most influential features identified by the Decision Tree were:

1. cp (Chest Pain Type)
2. oldpeak
3. ca
4. age
5. trestbps

These features contributed the most to the prediction of heart disease.

---

##  Overfitting Analysis

The initial model showed signs of overfitting with:

```text
Training Accuracy = 100%
Testing Accuracy  = 73%
```

To reduce overfitting, the tree depth was controlled using:

```python
max_depth = 3
```

After tuning:

```text
Training Accuracy = 84.64%
Testing Accuracy  = 75.41%
```

This resulted in a more balanced and generalized model.

---

##  Conclusion

A Decision Tree Classifier was successfully developed to predict heart disease. The model achieved approximately 75% testing accuracy while maintaining balanced precision, recall, and F1-score values. Feature importance analysis showed that Chest Pain Type, oldpeak, and ca were the most significant predictors. The project demonstrates a complete machine learning workflow from data preprocessing to model evaluation.

---

##  Future Improvements

* Random Forest Classifier
* Hyperparameter Tuning with GridSearchCV
* Cross Validation
* XGBoost
* Deployment using Streamlit

---

##  Author

Gautam Giria

Computer Science Engineering Student | Aspiring AI & Machine Learning Engineer
