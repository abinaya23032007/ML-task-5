# EV Car Price Prediction using Machine Learning

## 📌 Project Overview

This project uses Machine Learning to predict the **price of electric cars in India** based on features such as brand, model, range, power, and battery capacity.

The project uses **Ridge Regression** along with data preprocessing techniques to build and evaluate the prediction model.

## 🎯 Objective

The main objective of this project is to:

* Analyze an electric vehicle dataset.
* Preprocess numerical and categorical data.
* Predict EV car prices.
* Compare different Ridge Regression `alpha` values.
* Evaluate the model using different performance metrics.

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Google Colab / Jupyter Notebook

## 📂 Dataset

The project uses:

`ev_car_India_dataset.csv`

The dataset contains information about electric cars in India.

### Features Used

**Categorical Features:**

* Brand
* Model

**Numerical Features:**

* Range
* Power
* Battery

**Target Variable:**

* Price

## 🔄 Machine Learning Workflow

1. Load the EV car dataset.
2. Explore the dataset using `head()`, `shape()`, and null-value checking.
3. Separate input features and the target variable.
4. Identify categorical and numerical columns.
5. Apply preprocessing:

   * `StandardScaler` for numerical features.
   * `OneHotEncoder` for categorical features.
6. Split the dataset into training and testing sets.
7. Apply Ridge Regression.
8. Test different `alpha` values.
9. Predict EV prices.
10. Evaluate the model using MAE, RMSE, and R².

The implementation uses a `ColumnTransformer` and `Pipeline` to combine preprocessing with Ridge Regression.

## 🤖 Model Used

### Ridge Regression

Ridge Regression is a linear regression technique that includes regularization to help control model complexity.

The project tests different values of `alpha`:

```text
0.01
0.1
10
100
```

## 📊 Model Evaluation

The model is evaluated using:

### Mean Absolute Error (MAE)

Measures the average absolute difference between actual and predicted prices.

### Root Mean Squared Error (RMSE)

Measures prediction error while giving greater weight to larger errors.

### R² Score

Shows how well the model explains the variation in the target price.

The project calculates these metrics for both the training and testing data.

## 📁 Project Structure

```text
EV-Car-Price-Prediction/
│
├── ML.ipynb
├── ml.py
├── ev_car_India_dataset.csv
└── README.md
```

## ▶️ How to Run

### 1. Install Required Libraries

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

### 2. Open the Project

You can run the project using:

* Google Colab
* Jupyter Notebook
* VS Code

### 3. Add the Dataset

Place `ev_car_India_dataset.csv` in the required project location.

### 4. Run the Code

Run `ML.ipynb` or execute:

```bash
python ml.py
```

## 📈 Output

The program displays:

* Dataset information
* Model predictions
* Training MAE
* Training RMSE
* Training R²
* Testing MAE
* Testing RMSE
* Testing R²
* Ridge Regression results for the selected `alpha` values

## 🔮 Future Improvements

* Add more EV features such as charging time and seating capacity.
* Try other regression algorithms.
* Perform cross-validation.
* Tune hyperparameters more systematically.
* Add visualizations for actual vs predicted prices.
* Deploy the model as a web application.


