# 🚕 Cab Fare Prediction: Machine Learning Approach

A complete end-to-end machine learning project that predicts cab fares based on ride features such as distance, time of day, weather conditions, and surge pricing. Built using real-world Uber and Lyft ride data from Boston, MA.

**Author:** Roshni Dodhi
**Date:** October 2025
**Project Type:** Supervised Learning — Regression

---

## 📌 Problem Statement

Ride-hailing fares fluctuate based on a wide range of factors — distance, demand, time, weather, and service tier. This project builds and compares regression models to accurately predict the fare (`price`) for a given cab ride, helping both riders and companies better understand pricing dynamics.

---

## 📂 Dataset

| Detail | Value |
|---|---|
| **Records** | 693,071 rides |
| **Features** | 57 columns |
| **Target Variable** | `price` (continuous) |
| **Cab Services** | Uber & Lyft |
| **Location** | Boston, MA (Nov–Dec 2018) |

Key feature categories include ride metadata (source, destination, distance, cab type, service name), temporal features (hour, day, month), surge pricing, and a rich set of weather variables (temperature, humidity, wind, precipitation, cloud cover, visibility, etc.).

---

## 🛠️ Project Workflow

1. **Data Loading & Initial Exploration** — Shape inspection, data types, summary statistics, and missing value assessment.
2. **Data Cleaning & Preprocessing** — Handling ~55K null prices, type conversions, and preparing features for modeling.
3. **Exploratory Data Analysis (EDA)** — Visualizing price distributions, correlations, temporal patterns, and Uber vs. Lyft comparisons using Matplotlib, Seaborn, and Plotly.
4. **Feature Engineering** — Encoding categorical variables, scaling numerical features, and selecting the most predictive columns.
5. **Model Building** — Training three regression models: Linear Regression, Decision Tree, and Random Forest.
6. **Model Evaluation** — Comparing models using R², MAE, and RMSE on both train and test sets.
7. **Conclusions & Business Recommendations**

---

## 📊 Model Results

| Model | R² Score | MAE | RMSE |
|---|---|---|---|
| Linear Regression | 0.9347 | $1.67 | $2.24 |
| **Decision Tree** | **0.9960** | **$0.30** | **$0.55** |
| Random Forest | 0.9594 | $1.28 | $1.76 |

**Best Model:** Decision Tree — explains 99.6% of fare variance with an average prediction error of just $0.30.

---

## 💡 Key Insights

- **Distance** and **surge multiplier** are the strongest predictors of fare price.
- Peak demand occurs during morning (7–9 AM) and evening (5–7 PM) rush hours; late-night rides also carry higher fares.
- **Weather** impacts pricing — rain and poor conditions correlate with increased demand and surge pricing.
- Uber and Lyft show different pricing strategies, with premium tiers (Lux, Black) significantly more expensive than shared rides.

---

## 🔧 Tech Stack

- **Language:** Python 3.13
- **Data:** Pandas, NumPy
- **Visualization:** Matplotlib, Seaborn, Plotly
- **Machine Learning:** Scikit-learn (LinearRegression, DecisionTreeRegressor, RandomForestRegressor)
- **Environment:** Jupyter Notebook

---

## 🚀 Getting Started

```bash
# Clone the repo
git clone https://github.com/your-username/cab-fare-prediction.git
cd cab-fare-prediction

# Install dependencies
pip install pandas numpy matplotlib seaborn plotly scikit-learn

# Run the notebook
jupyter notebook Cab_Analysis_Final.ipynb
```

---

## 📁 Project Structure

```
cab-fare-prediction/
├── Cab_Analysis_Final.ipynb   # Main analysis notebook
├── README.md                  # Project documentation
└── data/                      # Dataset directory (add your CSV here)
```

---

## 🔮 Future Improvements

- Incorporate real-time traffic data
- Add event calendar features (sports games, concerts)
- Include driver availability and user ratings
- Experiment with deep learning and gradient boosting models (XGBoost, LightGBM)

---

## 📝 License

This project is for educational and portfolio purposes.
