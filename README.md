# 🏠 House Price Prediction Using Simple Linear Regression

## 📌 Project Overview

This project demonstrates how to predict house prices using **Simple Linear Regression (SLR)** with Python and Scikit-learn. The model uses **Square Footage** as the independent variable and **House Price** as the dependent variable.

The goal is to understand the relationship between a house's size and its market value, and to build a regression model capable of estimating house prices based on square footage.

---

## 🎯 Objectives

* Perform data preprocessing and exploration.
* Split the dataset into training and testing sets.
* Train a Simple Linear Regression model.
* Evaluate model performance using R² Score and RMSE.
* Visualize the regression line and data points.
* Predict house prices for unseen data.

---

## 📂 Dataset

The dataset contains the following columns:

| Feature        | Description                      |
| -------------- | -------------------------------- |
| Square_Footage | Area of the house in square feet |
| House_Price    | Price of the house               |

### Target Variable

* **House_Price**

### Input Feature

* **Square_Footage**

---

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* Jupyter Notebook

---

## 📊 Machine Learning Workflow

### 1. Import Libraries

Load the required Python libraries for data manipulation, visualization, and machine learning.

### 2. Load Dataset

Read the dataset using Pandas.

### 3. Feature Selection

```python
X = df[['Square_Footage']]
y = df['House_Price']
```

### 4. Train-Test Split

Split the dataset into training and testing sets.

```python
train_test_split(
    X, y,
    test_size=0.3,
    random_state=45
)
```

### 5. Model Training

Train a Simple Linear Regression model.

```python
from sklearn.linear_model import LinearRegression

reg = LinearRegression()
reg.fit(X_train, y_train)
```

### 6. Prediction

Generate predictions on both training and testing datasets.

### 7. Model Evaluation

Evaluate performance using:

* R² Score (Accuracy Measure)
* Root Mean Squared Error (RMSE)

```python
r2_score()
root_mean_squared_error()
```

### 8. Visualization

Plot:

* Training Data vs Regression Line
* Testing Data vs Regression Line

---

## 📈 Performance Metrics

### R² Score

Measures how well the model explains the variance in house prices.

* Value close to **1** → Excellent fit
* Value close to **0** → Poor fit

### RMSE

Measures prediction error.

* Lower RMSE indicates better model performance.

---

## 📉 Visualization Output

The notebook generates scatter plots showing:

1. Training data with fitted regression line.
2. Testing data with predicted regression line.

These visualizations help understand the linear relationship between house size and price.

---

## 🚀 How to Run

1. Clone the repository:

```bash
git clone https://github.com/Teja1444
```

2. Install dependencies:

```bash
pip install pandas numpy matplotlib scikit-learn
```

3. Open Jupyter Notebook:

```bash
jupyter notebook
```

4. Run all cells in:

```text
house_price_regression_data.ipynb
```

---

## 📋 Project Structure

```text
├── house_price_regression_data.ipynb
├── house_price_regression_dataset.csv
├── README.md
```

---

## 🔮 Future Improvements

* Multiple Linear Regression with additional features.
* Feature engineering and data preprocessing.
* Hyperparameter tuning.
* Model comparison with Decision Tree and Random Forest Regressors.
* Interactive web application using Streamlit.

---

## 👨‍💻 Author

Developed as a Machine Learning project to demonstrate the implementation of Simple Linear Regression for house price prediction using Python and Scikit-learn.
