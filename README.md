# 🌾 Fertilizer Recommendation System using Machine Learning

This project predicts the most suitable fertilizer type based on environmental and soil conditions. It uses classification algorithms such as **Logistic Regression**, **Random Forest**, and **CatBoost**, enhanced with **feature engineering**, **data preprocessing**, and **model evaluation using cross-validation**.

---

## 📊 Problem Statement

Farmers often struggle to determine the best fertilizer for their crops, which can lead to over- or under-application, affecting yield and soil health. This system aims to automate and optimize fertilizer recommendations based on:

- Soil nutrient composition (Nitrogen, Phosphorous, Potassium)
- Environmental factors (Temperature, Humidity, Moisture)
- Categorical features (Soil type, Crop type)

---



## 🛠️ Features

- ✅ Cleaned and preprocessed both training and testing datasets
- ✅ Engineered domain-specific features (e.g., NPK ratios, temperature levels)
- ✅ Applied label encoding and one-hot encoding
- ✅ Used `train_test_split` and `StandardScaler`
- ✅ Trained and evaluated three classifiers
  - Logistic Regression
  - Random Forest Classifier
  - CatBoost Classifier
- ✅ Compared models using `cross_val_score` with accuracy scoring
- ✅ Selected the best-performing model based on mean accuracy

---

## 🔍 Feature Engineering Highlights

- `Temp_Humid`: Interaction between temperature and humidity
- `Moisture_Nitrogen`: Combined soil moisture and nitrogen level
- `NPK_Sum` and `NPK_Mean`: Aggregate and average NPK values
- `N_P_Ratio`, `K_P_Ratio`: Fertilizer-specific ratios
- Polynomial transformations: `Temperature^2`, `Moisture^3`
- Binned categories: `Temp_Level`, `Moisture_Level`

---

## 🧠 Model Evaluation

Each model was evaluated using 5-fold cross-validation:

| Model                | Mean Accuracy      |
|---------------------|---------------------|
| Logistic Regression | 0.16012833333333332 |
| Random Forest       | 0.174885            |
| CatBoost            | 0.17734666666666668 |


---

## 🔧 Installation

```bash
git clone https://github.com/yourusername/fertilizer-recommender.git
cd fertilizer-recommender
pip install -r requirements.txt
```

---


---
▶️ Usage
You can run the notebook:

```bash
jupyter notebook notebooks/fertilizer_classification.ipynb
```

---


---
📌 Requirements:
- Python 3.8+

- pandas

- numpy

- scikit-learn

- catboost

- matplotlib / seaborn (for visuals)

---

🤝 Contributing
Pull requests are welcome! If you want to contribute major changes, please open an issue first to discuss what you would like to change.

📜 License
This project is licensed under the MIT License.

✨ Acknowledgments
- Kaggle / Data provider for the dataset

- scikit-learn and CatBoost for robust modeling tools

