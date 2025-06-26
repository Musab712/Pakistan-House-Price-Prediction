## 🏡 Pakistan House Price Prediction

A machine learning project that predicts house prices in Pakistan based on location, property type, area, and other key features. The project includes exploratory data analysis, feature engineering, model building, and evaluation — achieving an accuracy of **83%**.

---

### 📌 Table of Contents

* [Project Overview](#project-overview)
* [Dataset](#dataset)
* [EDA Highlights](#eda-highlights)
* [Preprocessing](#preprocessing)
* [Modeling](#modeling)
* [Results](#results)
* [Technologies Used](#technologies-used)
* [How to Run](#how-to-run)
* [Future Improvements](#future-improvements)
* [Author](#author)

---

### 📖 Project Overview

This project aims to predict house prices in Pakistan using supervised machine learning techniques. The dataset includes real-world features such as:

* City
* Province
* Property Type
* Purpose (Rent/Sale)
* Area (TotalArea)
* Baths, Bedrooms
* Latitude & Longitude
* Agency and Agent info

---

### 📂 Dataset

The dataset is collected from a real estate source and includes \~20,000 property listings from cities like Karachi, Lahore, Islamabad, and others.

**Key Columns:**

* `Price` *(Target)*
* `City`, `ProvinceName`, `PropertyType`, `Purpose`
* `TotalArea`, `Bedrooms`, `Baths`
* `Latitude`, `Longitude`

---

### 📊 EDA Highlights

* Price is heavily skewed; log transformation applied.
* Karachi has the highest concentration of listings.
* Boxplots and KDE plots used to analyze price distributions.
* Price varies significantly by **City**, **Property Type**, and **Purpose**.

---

### 🔧 Preprocessing

* Missing values handled using appropriate imputation
* Categorical features encoded with `LabelEncoder`
* Numerical features standardized using `StandardScaler`

---

### 🤖 Modeling

Tried multiple regression models:

* ✅ Linear Regression
* ✅ Random Forest Regressor
* ✅ SVR
* ✅ KNN Regressor

Best performing model: **Gradient Boosting Regressor**
**Accuracy (R² Score):** **83%**

---

### 📈 Results

| Metric   | Score         |
| -------- | ------------- |
| R² Score | 0.83          |
| RMSE     | \~850,000 PKR |
| MAE      | \~600,000 PKR |

---

### 🛠 Technologies Used

* Python 🐍
* Pandas, NumPy
* Scikit-learn
* Matplotlib, Seaborn
* Jupyter Notebook

---

### ▶️ How to Run

1. Clone the repo:

   ```bash
   git clone https://github.com/yourusername/pakistan-house-price-prediction.git
   cd pakistan-house-price-prediction
   ```

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Run the Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

4. Open and run `House_Price_Prediction.ipynb`

---

### 🔮 Future Improvements

* Use XGBoost/LightGBM for better performance
* Deploy model with a Streamlit web app
* Add geospatial visualizations for latitude/longitude
* Use deep learning with TensorFlow/Keras


