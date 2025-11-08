
# 🏠 House Price Prediction using TensorFlow

A **neural network regression model** to predict house prices based on key features such as size, bedrooms, age, and location.

---

## 📋 Project Overview

- **Model Type:** Regression Neural Network  
- **Features:** Size (sqft), Bedrooms, Age, Location  
- **Target:** House Price (in Thousands → converted to Lakhs for output)  
- **Frameworks:** TensorFlow / Keras  
- **Dataset:** Custom CSV file (`house_prices.csv`)

This project demonstrates a complete ML workflow — from preprocessing and model training to evaluation and manual prediction.

---

## 🚀 Quick Start

### 1. Install dependencies
```bash
pip install -r requirements.txt
````

### 2. Run the notebook

```bash
jupyter notebook House_Price_Prediction.ipynb
```

### 3. Execute all cells to:

* Load and preprocess data
* Train and evaluate the neural network
* Visualize results
* Predict house prices manually

---

## 📊 Dataset

**File:** `house_prices.csv`

| Column      | Description                                                       |
| ----------- | ----------------------------------------------------------------- |
| `size_sqft` | House size in square feet                                         |
| `bedrooms`  | Number of bedrooms                                                |
| `age`       | Age of the house in years                                         |
| `location`  | City (Chennai, Delhi, Hyderabad, Kochi, etc.)                     |
| `price`     | House price in **thousands** (converted to lakhs for predictions) |

---

## 🧠 Model Architecture

```python
Sequential([
    Dense(64, activation='relu', input_shape=(X_train.shape[1],)),
    Dense(32, activation='relu'),
    Dense(1)  # Output layer for regression
])
```

* **Optimizer:** Adam
* **Loss:** Mean Squared Error
* **Metric:** Mean Absolute Error (MAE)
* **Epochs:** 100

---

## 📈 Results

* **Mean Absolute Error:** ~7–10 Thousand (≈ 0.07–0.10 Lakhs)
* **Evaluation Metric:** MAE on Test Set
* **Visualizations:**

  * Feature correlation heatmap
  * Actual vs Predicted price scatter plot
  * Distribution of errors

---

## 💡 Example Prediction

```python
# Manual Prediction Example
Input:
  Size: 1800 sqft
  Bedrooms: 3
  Age: 10 years
  Location: Delhi

Output:
  🏠 Predicted House Price: 1.28 Lakhs
```

*(Note: The model predicts in thousands and is converted to lakhs by dividing by 100.)*

---

## 📁 Files Included

| File                           | Description                            |
| ------------------------------ | -------------------------------------- |
| `House_Price_Prediction.ipynb` | Main notebook containing full workflow |
| `house_prices.csv`             | Dataset used for model training        |
| `requirements.txt`             | List of Python dependencies            |

---

## 👨‍💻 Author

**Aravind R Nair**

---

*Simple and effective house price prediction using deep learning (predictions shown in Lakhs).*

