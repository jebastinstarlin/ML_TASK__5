# 🚗 ML Task 5 – EV Car Price Prediction Using Ridge Regression

## 📌 Project Overview

This project focuses on predicting the **price of electric vehicles (EVs) in India** using **Ridge Regression**.

The model uses important vehicle specifications such as:

* **Brand**
* **Model**
* **Range**
* **Power**
* **Battery**

The **Price** of the EV is used as the target variable for prediction.

---

## 🎯 Project Objectives

The main objectives of this project are:

* Explore and understand the EV dataset.
* Identify categorical and numerical features.
* Handle data preprocessing.
* Encode categorical variables using **One-Hot Encoding**.
* Scale numerical features using **StandardScaler**.
* Split the dataset into training and testing sets.
* Build a **Ridge Regression** model.
* Experiment with different `alpha` values.
* Evaluate model performance using regression metrics.

---

## 📂 Dataset

**Dataset Name:** EV Car India Dataset

The dataset contains information about electric vehicles available in the Indian market.

### 📊 Features

| Feature   |  Data Type  | Description                     |
| :-------- | :---------: | :------------------------------ |
| `Brand`   | Categorical | Manufacturer or brand of the EV |
| `Model`   | Categorical | Specific EV model               |
| `Range`   |  Numerical  | Driving range of the vehicle    |
| `Power`   |  Numerical  | Power output of the vehicle     |
| `Battery` |  Numerical  | Battery capacity                |
| `Price`   |    Target   | Price of the electric vehicle   |

---

## 🛠️ Technologies & Libraries

* **Python**
* **Pandas**
* **NumPy**
* **Matplotlib**
* **Seaborn**
* **Scikit-learn**
* **Google Colab**
* **Jupyter Notebook**

---

## 🔄 Machine Learning Workflow

```text
Import Dataset
      ↓
Explore & Understand Data
      ↓
Check Missing Values
      ↓
Define Features & Target
      ↓
Identify Categorical & Numerical Features
      ↓
Apply One-Hot Encoding
      ↓
Scale Numerical Features
      ↓
Split Data into Training & Testing Sets
      ↓
Build Ridge Regression Model
      ↓
Experiment with Alpha Values
      ↓
Evaluate Model Performance
```

---

## ⚙️ Data Preprocessing

The dataset is divided into **input features (`X`)** and the **target variable (`y`)**.

### 🔤 Categorical Features

The following categorical features are used:

* `Brand`
* `Model`

These features are converted into numerical values using **OneHotEncoder**.

### 🔢 Numerical Features

The following numerical features are used:

* `Range`
* `Power`
* `Battery`

These features are standardized using **StandardScaler**.

### 🔧 ColumnTransformer

A **ColumnTransformer** is used to apply the appropriate preprocessing technique to each type of feature:

```text
Categorical Features → OneHotEncoder
Numerical Features   → StandardScaler
```

This ensures that each feature is processed appropriately before training the model.

---

## 🤖 Machine Learning Model

### Ridge Regression

The project uses **Ridge Regression**, which is a regularized version of Linear Regression.

Ridge Regression adds a regularization term to the loss function to reduce the impact of large model coefficients and help prevent overfitting.

### 🔧 Alpha Values

The following `alpha` values are tested:

```text
0.01
0.1
1
10
100
```

The `alpha` parameter controls the strength of regularization.

* Lower `alpha` → weaker regularization
* Higher `alpha` → stronger regularization

Testing multiple values helps determine how regularization affects model performance.

---

## 📊 Model Evaluation

The trained model is evaluated using the following regression metrics:

### 1. MAE – Mean Absolute Error

MAE measures the average absolute difference between the actual and predicted EV prices.

**Lower MAE indicates smaller prediction errors.**

### 2. RMSE – Root Mean Squared Error

RMSE measures the prediction error while giving greater importance to larger errors.

**Lower RMSE indicates better prediction performance.**

### 3. R² Score

R² Score indicates how well the model explains the variation in EV prices.

A value closer to **1** generally indicates that the model explains more of the variation in the target variable.

---

## 🚀 How to Run the Project

### ☁️ Using Google Colab

1. Open the `.ipynb` notebook in **Google Colab**.
2. Upload the EV dataset.
3. Make sure the CSV filename matches the filename used in the notebook.
4. Run the notebook cells sequentially.
5. Review the data preprocessing steps.
6. Train the Ridge Regression model.
7. Compare the results for different `alpha` values.
8. Analyze the MAE, RMSE, and R² Score.

### 💻 Local Environment

Install the required Python libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

Then open the notebook using **Jupyter Notebook** or **JupyterLab**.

---

## 📁 Project Structure

```text
ML-Task-5/
│
├── ML_NTask_5.ipynb
├── ev_car_India_dataset.csv
└── README.md
```

---

## 📈 Key Learning Outcomes

This project demonstrates the following machine learning concepts:

* Exploratory Data Analysis (EDA)
* Feature and target separation
* Categorical feature encoding
* Numerical feature scaling
* `ColumnTransformer`
* Train-Test Split
* Machine Learning Pipelines
* Ridge Regression
* Hyperparameter experimentation
* Model regularization
* Regression model evaluation
* MAE, RMSE, and R² Score

---

## ✅ Conclusion

This project demonstrates an end-to-end machine learning workflow for **predicting EV prices using Ridge Regression**.

The project covers:

**Data Exploration → Preprocessing → Feature Encoding → Feature Scaling → Model Training → Hyperparameter Experimentation → Model Evaluation**

It provides a practical example of applying **supervised machine learning** to an **electric vehicle price prediction problem** using real-world vehicle specifications.
