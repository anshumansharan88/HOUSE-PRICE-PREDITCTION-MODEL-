# HOUSE-PRICE-PREDITCTION-MODEL-
A Machine Learning regression project that predicts California house price prediction using Scikit-Learn, including data preprocessing, feature engineering, Random Forest, cross-validation and hyperparameter tuning

# 🏠 House Price Prediction Model

An end-to-end **Machine Learning regression project** that predicts median house prices in California using **Scikit-Learn**.

The project covers data exploration, preprocessing, feature engineering, model training, evaluation, cross-validation, and hyperparameter tuning using **Grid Search and Randomized Search**.

---

## 📌 Project Overview

The objective of this project is to build a Machine Learning model that can predict the **median house value** of a California housing district based on various demographic and geographical features.

This project follows a complete Machine Learning workflow, from understanding the dataset to tuning the final model.

---

## 📊 Dataset

The project uses the **California Housing Dataset**.

The dataset contains information about different districts in California.

### Features

| Feature              | Description                    |
| -------------------- | ------------------------------ |
| `longitude`          | Longitude of the district      |
| `latitude`           | Latitude of the district       |
| `housing_median_age` | Median age of houses           |
| `total_rooms`        | Total number of rooms          |
| `total_bedrooms`     | Total number of bedrooms       |
| `population`         | Population of the district     |
| `households`         | Number of households           |
| `median_income`      | Median income of households    |
| `ocean_proximity`    | Location relative to the ocean |
| `median_house_value` | Target variable                |

---

## 🔄 Machine Learning Workflow

```text
Dataset
   ↓
Data Exploration & Visualization
   ↓
Train/Test Split
   ↓
Stratified Sampling
   ↓
Data Cleaning
   ↓
Missing Value Imputation
   ↓
Feature Engineering
   ↓
Categorical Encoding
   ↓
Feature Scaling
   ↓
Model Training
   ↓
Cross-Validation
   ↓
Hyperparameter Tuning
   ↓
Final Model Evaluation
```

---

## 🧹 Data Preprocessing

Several preprocessing techniques were implemented using Scikit-Learn.

### Missing Values

Missing values in numerical features were handled using:

```python
SimpleImputer(strategy="median")
```

### Categorical Features

The `ocean_proximity` feature was converted into numerical values using:

```python
OneHotEncoder()
```

### Feature Scaling

Numerical features were standardized using:

```python
StandardScaler()
```

### Preprocessing Pipeline

`Pipeline` and `ColumnTransformer` were used to combine the preprocessing steps into a structured workflow.

---

## 🤖 Machine Learning Models

The following regression models were explored:

### Linear Regression

Used as a baseline regression model.

### Decision Tree Regressor

Used to capture non-linear relationships between the features and target variable.

### Random Forest Regressor

A Random Forest model was used as the primary ensemble approach.

The Random Forest model was further optimized using hyperparameter tuning.

---

## 🔍 Hyperparameter Tuning

Two Scikit-Learn techniques were explored:

### Grid Search

`GridSearchCV` was used to evaluate predefined combinations of hyperparameters using cross-validation.

Parameters explored included:

* `n_estimators`
* `max_features`
* `bootstrap`

### Randomized Search

`RandomizedSearchCV` was also implemented to explore a randomized selection of hyperparameter combinations.

This provides an efficient alternative to testing every possible combination in a large parameter search space.

---

## 📏 Model Evaluation

The models were evaluated using **Root Mean Squared Error (RMSE)**.

RMSE measures the average magnitude of prediction errors, with larger errors receiving more weight.

```text
RMSE = √(Mean Squared Error)
```

**Lower RMSE = Better model performance**

Cross-validation was also used to obtain a more reliable estimate of model performance.

---

## 🛠️ Technologies & Libraries

* Python
* NumPy
* Pandas
* Matplotlib
* Scikit-Learn
* Jupyter Notebook

---

## 📁 Project Structure

```text
House-Price-Prediction/
│
├── .gitignore
├── LICENSE
├── README.md
├── requirements.txt
└── house_price_prediction.ipynb
```

> The exact structure may vary depending on the files included in the repository.

---

## 📚 Key Concepts Learned

This project helped me understand and implement:

* Exploratory Data Analysis
* Train/Test Splitting
* Stratified Sampling
* Data Cleaning
* Missing Value Imputation
* Feature Engineering
* Categorical Encoding
* Feature Scaling
* Scikit-Learn Pipelines
* ColumnTransformer
* Regression Models
* Cross-Validation
* RMSE
* GridSearchCV
* RandomizedSearchCV
* Hyperparameter Tuning

---

## 🔮 Future Improvements

* Deploy the trained model using **FastAPI or Streamlit**
* Create an interactive prediction interface
* Experiment with additional regression algorithms
* Perform advanced feature engineering
* Compare additional hyperparameter optimization techniques
* Monitor model performance after deployment

---

## 📖 Reference

This project was developed as part of my Machine Learning learning journey using concepts from:

**Hands-On Machine Learning with Scikit-Learn, Keras & TensorFlow**
by **Aurélien Géron**

---

## 👨‍💻 Author

**Anshuman Sharan**

B.Tech CSE — Data Science

Interested in **Data Science, Machine Learning, Data Analytics, and AI**.

---

⭐ If you found this project useful, consider giving the repository a star!
