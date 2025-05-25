## **README.md**

# 🏡 House Price Prediction 

This project aims to predict house prices using various machine learning models, including **Linear Regression, Linear Regression (with log-transformed target)**, **Random Forest**, **Random Forest (Tuned)** , **XGBoost**, **LightGBM**, **Gradient Boosting**, and **Extra Trees**.

The best-performing model in this project was **Linear Regression (Log-Transformed)**, which achieved the lowest RMSE.


## 📊 Dataset

**Source:** [Kaggle- House Price Prediction](https://www.kaggle.com/datasets/zafarali27/house-price-prediction-dataset)

**Details:** The dataset contains **2,000 house records** with the following features:
- `Id` — unique identifier
- `Area` — size of the house (in square feet)
- `Bedrooms` — number of bedrooms
- `Bathrooms` — number of bathrooms
- `Floors` — number of floors
- `YearBuilt` — year the house was built
- `Location` — encoded as categorical (Downtown, Urban, Suburban, Rural)
- `Condition` — encoded as categorical (Fair, Excellent, Poor, Good)
- `Garage` — encoded as binary (Yes/No)
- `Price` — target variable (house price in currency)

---

## ⚙️ Models Trained

| Model                                   | RMSE (lower is better)  | R² Score          |
|-----------------------------------------|--------------------------|-------------------|
| Linear Regression (Log-Transformed)     | ✅ Best (~0.75, log scale) | Slightly negative |
| Random Forest (Tuned)                   | ~280,000                | Negative          |
| Linear Regression (Raw)                 | ~280,000                | Negative          |
| Gradient Boosting                       | ~283,000                | Negative          |
| LightGBM                                | ~298,000                | Negative          |
| Extra Trees                             | ~315,000                | Negative          |
| XGBoost                                 | ~324,000                | Negative          |

*Note: The log-transformed model showed the best generalization.*

---

## 🏗️ Project Structure

```

├── Dataset/
│   └── house price prediction dataset.csv
├── notebooks/
│   └── house price prediction.ipynb
├── Best model/
│   └── linear regression log model.pkl
├── README.md
├── requirement.txt
````

---

### Clone the Repository

```bash
git clone https://github.com/vaibhavi1224/house-price-prediction.git
cd house-price-prediction
````
Install the required dependencies:

```bash
pip install -r requirements.txt
```

Launch the Jupyter Notebook:

```bash
jupyter notebook house-price-prediction.ipynb
```


---

### 📦 requirements.txt (if you need)


Here’s a minimal `requirements.txt`:
```
numpy
pandas
scikit-learn
joblib
xgboost
lightgbm
matplotlib
seaborn
```

## 💬 Contact

If you have questions, suggestions, or want to collaborate:

**Vaibhavi Kapse**

[GitHub](https://github.com/vaibhavi1224) | [LinkedIn](https://linkedin.com/in/vaibhavi-kapse-1224work) | [Email](kapsevaibhavi1224@gmail.com)


## 🌟 Star this repository if you find it helpful!

---
