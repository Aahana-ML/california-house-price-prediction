# 🌴🏡 California House Price Prediction

🚀 **[Live Demo — California House Price Estimator](https://california-house-price-estimate.streamlit.app/)**

An end-to-end Machine Learning project that predicts the median house price of California districts using an XGBoost regression model.

The project includes exploratory data analysis (EDA), model comparison, feature importance analysis, and an interactive Streamlit web application for real-time predictions.


## 🎯 Problem Statement

The objective of this project is to predict the median house price of a California district based on demographic, geographic, and housing-related features.

Instead of relying on manual estimation, the machine learning model learns patterns from historical housing data and generates predictions for new districts entered by the user.


## 📂 Dataset

This project uses the California Housing Dataset provided by Scikit-Learn.

### Features

- Median Income
- House Age
- Average Rooms
- Average Bedrooms
- Population
- Average Occupancy
- Latitude
- Longitude

### Target

- Median House Value (in hundreds of thousands of dollars)


## 🤖 Machine Learning Models

The following regression models were trained and compared:

- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor
- XGBoost Regressor (Final Model)

XGBoost achieved the best overall performance and was selected for deployment.


## 📈 Model Performance

| Model | R² Score |
|--------|---------:|
| Linear Regression | 0.576 |
| Decision Tree | 0.623 |
| Random Forest | 0.805 |
| **XGBoost** | **0.837** |


## 📊 Feature Importance

The XGBoost model provides feature importance scores, allowing us to understand which variables contributed the most to predictions.

The model relies most heavily on:

1. Median Income
2. Average Occupancy
3. Longitude
4. Latitude

These insights improve model interpretability and explainability.


## 🛠️ Tech Stack

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-Learn
- XGBoost
- Joblib
- Streamlit


## ⚙️ Installation

Clone the repository

```bash
git clone <git remote add origin https://github.com/Aahana-ML/california-house-price-prediction.git>
```

Install dependencies

```bash
pip install -r requirements.txt
```


## ▶️ Running the Application

```bash
streamlit run app/app.py
```

The application will be available at:

```
http://localhost:8503/
```


## 🔮 Future Improvements

- Hyperparameter tuning using Optuna
- Model deployment on Streamlit Community Cloud
- SHAP explainability
- Interactive visualizations
- User input validation
- Docker containerization


## 🤝 Acknowledgements

This project was developed with guidance from ChatGPT for conceptual understanding, debugging, and project refinement.