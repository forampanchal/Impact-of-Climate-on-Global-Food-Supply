# 🌍 Impact of Climate Change on Global Food Supply

This project investigates how climate change affects global food security by analyzing historical crop yield, climate, and environmental data using machine learning models. We explore how changing temperatures, rainfall patterns, and CO₂ emissions are impacting agriculture, and we propose predictive models that help forecast future outcomes.

## 📌 Project Overview

As climate-driven events such as droughts, floods, and heatwaves become more frequent, their impact on food systems is growing. Our goal is to develop machine learning models that help forecast changes in crop yields based on environmental variables, allowing communities and policymakers to better plan for food resilience.

## 🧠 Machine Learning Models Used

We implemented and compared three models:

- **XGBoost:** Offered the highest accuracy (R² = 0.982, RMSE = 0.87). It effectively handled non-linear relationships and highlighted key features like rainfall and temperature as top yield predictors.
- **Decision Tree Regressor:** Simple and interpretable with strong performance (R² = 0.981). Useful for identifying key decision points but prone to overfitting.
- **LSTM (Long Short-Term Memory):** Captured time-based patterns in sequential data with moderate accuracy (R² = 0.774). Ideal for detecting long-term climate trends, though computationally heavy.

## 🧾 Dataset

- **FAOSTAT:** Crop yield, pesticide use, population (1970–2023)  
- **World Bank Data:** Annual precipitation and temperature  
- **IPCC Reports:** Global climate indicators and emissions data  

## ⚙️ Methodology

- Data cleaning and preprocessing: handled missing values, feature scaling, and one-hot encoding
- Feature engineering: temperature, rainfall, CO₂ emissions, pesticide use, and population
- Train-test split with model tuning (grid search for XGBoost)
- Evaluation using R² and RMSE for regression tasks

## 📈 Key Results

| Model               | R² Score | RMSE  |
|--------------------|----------|-------|
| XGBoost            | 0.982    | 0.87  |
| Decision Tree      | 0.981    | 1.45  |
| LSTM               | 0.774    | 1.12  |

XGBoost emerged as the best performer due to its robustness with large, complex datasets and high interpretability through feature importance.

## 💡 Future Work

- Incorporate satellite imagery and soil quality data
- Extend to region-specific or crop-specific models
- Experiment with advanced deep learning methods like CNNs and Transformers
- Integrate real-time monitoring using IoT for precision agriculture



