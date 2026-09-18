# Practical Machine Learning using Scikit-learn

## 📌 Project Overview

This project is a practical implementation of Machine Learning using Python and Scikit-learn.

The main project focuses on predicting **median house values using the California Housing Dataset**. It covers the complete Machine Learning workflow, starting from data preparation and feature engineering to model training, evaluation, cross-validation, model saving, and making predictions on new data.

The project also includes Iris training and testing datasets for practicing classification-based Machine Learning concepts.

---

## 🎯 Objectives

- Understand the complete Machine Learning workflow
- Work with real-world datasets
- Perform data preprocessing and feature engineering
- Handle missing values
- Work with numerical and categorical features
- Split data into training and testing sets
- Train different Machine Learning models
- Compare model performance
- Use cross-validation for evaluation
- Save a trained Machine Learning model
- Use the saved model to make predictions on new data

---

## 📊 Main Project: California Housing Price Prediction

The main dataset used in this project is the **California Housing Dataset**.

The objective is to predict the `median_house_value` of a district using different housing and geographical features.

### Features include:

- Longitude
- Latitude
- Housing Median Age
- Total Rooms
- Total Bedrooms
- Population
- Households
- Median Income
- Ocean Proximity

### Target Variable

**Median House Value**

This makes the project a **Supervised Learning Regression problem**.

---

## 🔄 Machine Learning Workflow

The project follows an end-to-end Machine Learning workflow:

**Data Collection → Data Exploration → Feature Engineering → Data Splitting → Data Preprocessing → Model Training → Cross-Validation → Model Evaluation → Model Saving → Prediction**

---

## 🧹 Data Preprocessing

Several preprocessing techniques are used to prepare the data for Machine Learning models.

### Missing Value Handling

Missing numerical values are handled using **median imputation**.

Categorical missing values are handled using the **most frequent value**.

### Feature Scaling

Numerical features are standardized using **StandardScaler**.

### Categorical Encoding

The categorical feature `ocean_proximity` is converted into numerical form using **One-Hot Encoding**.

### ColumnTransformer

Different preprocessing techniques are applied to numerical and categorical columns using **ColumnTransformer**.

---

## 🛠️ Feature Engineering

An `income_cat` feature is created from the `median_income` attribute.

The income values are divided into different categories to help perform **stratified sampling**.

This helps maintain a similar distribution of income categories in the training and testing datasets.

---

## 🔀 Stratified Sampling

The project uses **StratifiedShuffleSplit** to divide the housing dataset into training and testing data.

A test size of **20%** is used.

A fixed random state is also used to make the split reproducible.

---

## 🤖 Machine Learning Models

The project explores multiple regression algorithms.

### Linear Regression

Used as a basic regression model and baseline for comparison.

### Decision Tree Regressor

Used to capture non-linear relationships between the features and the target variable.

### Random Forest Regressor

Uses multiple decision trees together to improve prediction performance.

The Random Forest model is also used in the model-saving and prediction workflow.

---

## 📈 Model Evaluation

The models are evaluated using **Root Mean Squared Error (RMSE)**.

The project also uses **10-Fold Cross-Validation** to obtain a more reliable estimate of model performance.

### Evaluation Concepts

- RMSE
- Cross-Validation
- Training Performance
- Prediction Error
- Model Comparison

A lower RMSE indicates lower prediction error.

---

## 💾 Model Persistence

The project demonstrates how a trained Machine Learning model can be saved and reused.

The trained model and preprocessing pipeline are saved using **Joblib**.

This allows the model to be loaded later without retraining it from scratch.

---

## 🔮 Prediction on New Data

The project includes a separate prediction workflow where new housing data can be processed using the saved preprocessing pipeline.

The trained Random Forest model is then used to generate predicted house values.

The prediction results are stored in an output dataset.

---

## 🌸 Iris Dataset

The repository also contains separate Iris training and testing datasets.

These files can be used to practice **classification** problems and understand the difference between regression and classification.

The Iris dataset contains measurements such as:

- Sepal Length
- Sepal Width
- Petal Length
- Petal Width
- Class

The classes include:

- Iris-setosa
- Iris-versicolor
- Iris-virginica

---

## 🧰 Tools & Technologies

### Programming Language
- Python

### Libraries
- NumPy
- Pandas
- Scikit-learn
- Joblib

### Development Environment
- Jupyter Notebook

### Machine Learning Techniques
- Supervised Learning
- Regression
- Classification
- Feature Engineering
- Data Preprocessing
- Stratified Sampling
- Cross-Validation
- Model Evaluation
- Model Persistence

---

## 📚 Scikit-learn Concepts Practiced

- Train/Test Split
- StratifiedShuffleSplit
- Pipeline
- ColumnTransformer
- SimpleImputer
- StandardScaler
- OneHotEncoder
- Linear Regression
- Decision Tree Regression
- Random Forest Regression
- Cross-Validation
- RMSE
- Model Prediction
- Model Saving and Loading

---

## 📁 Project Files

### Notebooks

**proj(1).ipynb**  
Main notebook containing the California Housing Machine Learning workflow, including preprocessing, model training and evaluation.

**proj2(1).ipynb**  
Notebook focused on saving/loading the trained model and using it to make predictions on new housing data.

### Datasets

**housing.csv**  
Main California Housing dataset used for training and experimentation.

**input - Copy(1).csv**  
Housing data containing input records and prediction-related results.

**iris-train(2).xlsx**  
Iris training dataset.

**iris-test(2).xlsx**  
Iris testing dataset.

---

## 🧠 Key Learning Outcomes

Through this project, the following concepts were practiced:

- Understanding an end-to-end Machine Learning project
- Preparing real-world data for Machine Learning
- Handling missing values
- Processing numerical and categorical data
- Creating preprocessing pipelines
- Performing stratified sampling
- Training different regression models
- Evaluating models using RMSE
- Applying cross-validation
- Understanding model performance
- Saving trained models
- Reusing trained models for prediction
- Working with both regression and classification datasets

---

## 🚀 Future Improvements

Possible improvements to the project include:

- Hyperparameter tuning
- GridSearchCV and RandomizedSearchCV
- Feature importance analysis
- More detailed model comparison
- Visualization of prediction errors
- Improving the prediction pipeline
- Building an interactive Machine Learning application
- Deploying the model using Streamlit or an API

---

## 👨‍💻 Author

Indraneel Bhattacharya

A practical Machine Learning project created to learn and implement the end-to-end Machine Learning workflow using Python and Scikit-learn.
