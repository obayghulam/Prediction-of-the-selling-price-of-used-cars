# 🚗 Prediction of Used Car Selling Prices

This project focuses on building a **machine learning model** to predict the **selling price** of used cars based on various attributes. Accurate price predictions help both buyers and sellers ensure fair and competitive pricing in the used car market.

---

## 📊 Project Overview

- **Objective:** Predict the selling price of used cars using historical data.
- **Techniques Applied:**
    - Exploratory Data Analysis (EDA)
    - Feature Engineering (creating 'Age' feature, encoding categorical variables, scaling numerical features)
    - Regression Models:  
        - Linear Regression (Baseline)
        - Ridge Regression (L2 Regularization)
        - Lasso Regression (L1 Regularization + Feature Selection)
        - Polynomial Regression (Degree 2 & 3 for non-linear relationships)
- **Performance Evaluation:** Compared models using MAE, MSE, RMSE, and R².

---

## 📂 Project Files

| File Name | Description |
|---|---|
| `Project -Copy1.ipynb` | Jupyter Notebook containing the full data exploration, preprocessing, modeling, and evaluation pipeline |
| `README.md` | Project documentation (this file) |

---

## 📦 Technologies Used

- Python
- Pandas & NumPy (Data handling)
- Matplotlib & Seaborn (Visualization)
- Scikit-learn (Regression Models & Evaluation)

---

## 🔬 Methodology

### Data Exploration
- Examined dataset features: Car_Name, Selling_Price, Present_Price, Kms_Driven, Fuel_Type, Seller_Type, Transmission, Owner, Year.
- Created new `Age` feature (Current Year - Year), then dropped `Year` to avoid multicollinearity.
- Encoded categorical features (Fuel_Type, Seller_Type, Transmission) using dummy variables.

### Models Explained
| Model | Explanation |
|---|---|
| Linear Regression | Baseline model assuming simple linear relationships |
| Ridge Regression | L2 regularization to reduce overfitting |
| Lasso Regression | L1 regularization, performing automatic feature selection |
| Polynomial Regression (Degree 2) | Captures non-linear patterns (best performance) |
| Polynomial Regression (Degree 3) | More flexibility, but suffered from overfitting |

---

## 📊 Model Comparison Results

| Model | Performance Summary |
|---|---|
| Linear Regression | Basic accuracy, good baseline |
| Ridge Regression | Controlled overfitting but no major accuracy improvement |
| Lasso Regression | Simplified the model by removing weak features |
| Polynomial Regression (Degree 2) | **Best performer** - balanced flexibility and generalization |
| Polynomial Regression (Degree 3) | Severe overfitting with poor generalization |

---

## 🚀 How to Run

1. Clone the repository.
2. Open `Project -Copy1.ipynb` in Jupyter Notebook.
3. Run all cells to reproduce the analysis, training, and evaluation.

---

## 📈 Example Visuals
- Price distribution plots
- Pairplots showing relationships between variables
- Model comparison charts (MAE, RMSE, R²)

---

## 📖 Future Work
- Test advanced models like Random Forest or XGBoost.
- Incorporate additional features (e.g., location, maintenance history).
- Package as a web tool where users can input car details and get a predicted price.

---

## 📜 License
This project is open-source and available for educational purposes.
