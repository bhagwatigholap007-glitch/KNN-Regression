# KNN Regression – Outlet Sales Prediction

## 📌 Project Overview

This project uses the **K-Nearest Neighbors (KNN) Regression** algorithm to predict outlet sales based on various product and outlet-related features.

The project includes data preprocessing, feature encoding, model training, hyperparameter tuning, and evaluation using regression metrics.

---

## 🎯 Objective

To develop a KNN Regression model that predicts **Item Outlet Sales** using a real-world dataset and evaluate its predictive performance using:

- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R² Score

---

## 📊 Dataset

The dataset contains information about products and their respective outlets.

### Target Variable

`Item_Outlet_Sales`

### Dataset Information

- **Rows:** 8,523
- **Columns:** 12
- Contains product, outlet, and sales-related attributes.

---

## 🔧 Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook
- Streamlit
- Pickle

---

## 🧹 Data Preprocessing

The following preprocessing steps were performed:

1. Handling missing values in `Item_Weight`
2. Encoding categorical variables
3. Converting categorical features into numerical form
4. Preparing input features and target variable
5. Splitting the dataset into training and testing sets
6. Scaling/preparing features for KNN Regression

---

## 🤖 Machine Learning Algorithm

### K-Nearest Neighbors Regression

KNN Regression predicts the target value by finding the nearest data points to a given input and calculating their contribution to the prediction.

The model was tuned to find a suitable value of `K` and other parameters for better predictive performance.

### Final Model

- Algorithm: KNN Regression
- Number of Neighbors: 7
- Distance Parameter: Manhattan distance (`p=1`)
- Train-Test Split: 80:20
- Random State: 42

---

## 📈 Model Performance

The final model achieved the following results on the test dataset:

| Metric | Result |
|---|---:|
| MAE | 772.36 |
| MSE | 1,222,702.36 |
| RMSE | 1,105.76 |
| R² Score | 0.5501 |

The R² score indicates that the model explains approximately **55% of the variation** in outlet sales on the test data.

---

## 📁 Project Structure

```text
KNN_Outlet_Sales_Regression/
│
├── KNN Regression.ipynb
├── KNN_reg_outlet_sales - KNN_reg_outlet_sales.csv
├── app.py
├── knn_regression_model.pkl
├── preprocessing.pkl
├── features.pkl
├── metrics.json
├── requirements.txt
└── README.md
