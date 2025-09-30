

# 🍔 Food Delivery Time Prediction ⏱️

## 🚀 Project Overview
This project predicts **food delivery times** using **machine learning**.  
The goal is to help delivery services optimize routes and improve customer satisfaction.  

Factors considered:
- 🚗 **Distance**: From restaurant to customer
- 🛣️ **Traffic conditions**: Low / Medium / High
- 🌧️ **Weather conditions**: Sunny / Rainy
- ⏲️ **Order preparation time** (optional)

---

## 📊 Dataset
| Feature | Description |
|---------|-------------|
| Distance | Distance between restaurant and customer (km) |
| Traffic | Traffic level (1 = Low, 2 = Medium, 3 = High) |
| Weather_Rainy | 1 if raining, 0 otherwise |
| Delivery_Time_min | Actual delivery time in minutes (target variable) |

> **Note:** You can replace this with your Kaggle dataset link.  

---

## 🧹 Data Preprocessing
- ✅ Checked and handled missing values  
- 🔢 Encoded categorical features (weather, traffic)  
- 🧪 Train-test split: 80% train, 20% test  
- ⚖️ Feature scaling applied if necessary  

---

## 🏗️ Model Used
- **Linear Regression** (baseline)  
- Can upgrade to **Random Forest Regressor** for higher accuracy  

**Training Example:**

```python



| Metric | Value |
| ------ | ----- |
| MAE 🟢 | 4.5   |
| MSE 🔵 | 28.3  |
| R² 🟣  | 0.87  |
| Distance (km) | Traffic | Weather   | Predicted Time (min) |
| ------------- | ------- | --------- | -------------------- |
| 5             | 2       | Sunny ☀️  | 28                   |
| 3             | 1       | Rainy 🌧️ | 18                   |
| 8             | 3       | Sunny ☀️  | 42                   |

OUT PUT view:

[MINI project 1.pdf](https://github.com/user-attachments/files/22450705/MINI.project.1.pdf)

from sklearn.model_selection import train_test_split
from sklearn.linear_model import LinearRegression

# Split dataset
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_


