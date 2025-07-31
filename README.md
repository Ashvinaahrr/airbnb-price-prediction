# 🏡 Airbnb Price Prediction

Predicting Airbnb listing prices using machine learning techniques based on real NYC data.

![GitHub last commit](https://img.shields.io/github/last-commit/Ashvinaahrr/airbnb-price-prediction)
![Made with Python](https://img.shields.io/badge/Made%20with-Python-blue?logo=python)
![License](https://img.shields.io/badge/license-MIT-green)

---

## 📌 Table of Contents

- [Overview](#overview)
- [Project Goals](#project-goals)
- [Tech Stack](#tech-stack)
- [Dataset](#dataset)
- [EDA & Visualizations](#eda--visualizations)
- [Modeling](#modeling)
- [Results](#results)
- [How to Run](#how-to-run)
- [Next Steps](#next-steps)

---

## 📖 Overview

This project explores real-world Airbnb listings in NYC to predict listing prices based on location, room type, availability, and more.

It’s designed to showcase skills in:

- Data cleaning
- Exploratory data analysis (EDA)
- Machine learning modeling
- Visualization
- Real-world insight generation

---

## 🎯 Project Goals

- Predict Airbnb listing prices from structured data
- Explore feature importance and business implications
- Compare multiple regression models (linear, tree-based, ensemble, etc.)
- Present the best-performing model clearly

---

## 🛠️ Tech Stack

- **Language**: Python 3.9
- **IDE**: VS Code / Jupyter Notebook
- **Libraries**: pandas, numpy, seaborn, matplotlib, scikit-learn, xgboost, folium

---

## 📊 Dataset

- Source: [Inside Airbnb NYC](http://insideairbnb.com/get-the-data.html)
- File used: `listings.csv`
- ~40,000 listings including features like:
  - Location (latitude/longitude)
  - Room type
  - Price
  - Availability
  - Reviews

---

## 📈 EDA & Visualizations

Key steps:
- Cleaning and filtering outliers
- Visualizing spatial distributions using **folium**
- Correlation heatmaps and boxplots to explore trends
- Distribution analysis of prices and availability

![example](./screenshots/price_map_preview.png) <!-- optional: include a map or chart -->

---

## 🤖 Modeling

We trained 6 different models:

| Model              | RMSE   | R² Score |
|-------------------|--------|----------|
| Random Forest      | 73.85  | 0.22     |
| XGBoost            | 74.03  | 0.22     |
| SVR                | 79.84  | 0.09     |
| Linear Regression  | 81.27  | 0.06     |
| Ridge Regression   | 81.42  | 0.05     |
| KNN Regressor      | 81.56  | 0.05     |

**Best Model**: Random Forest

📌 Final prediction vs actual plot:

*(Include the actual plot image if you can!)*

---

## 💻 How to Run

1. Clone this repo:
```bash
git clone https://github.com/Ashvinaahrr/airbnb-price-prediction.git
