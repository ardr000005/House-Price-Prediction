# 🏠 House Price Prediction using TensorFlow

A neural network model to predict house prices based on features like size, bedrooms, age, and location.

## 📋 Project Overview

- **Model Type**: Regression Neural Network
- **Features**: Size (sqft), Bedrooms, Age, Location
- **Target**: House Price (in Lakhs)
- **Framework**: TensorFlow/Keras

## 🚀 Quick Start

1. **Install dependencies**:
```bash
pip install -r requirements.txt
```

2. **Run the notebook**:
```bash
jupyter notebook House_Price_Prediction.ipynb
```

3. **Execute all cells** to:
   - Load and preprocess data
   - Train the neural network
   - Evaluate model performance
   - Make predictions

## 📊 Dataset

`house_prices.csv` contains:
- `size_sqft`: House size in square feet
- `bedrooms`: Number of bedrooms
- `age`: House age in years
- `location`: City (Chennai, Delhi, Hyderabad, Kochi, etc.)
- `price`: Price in lakhs

## 🧠 Model Architecture

```python
Sequential([
    Dense(64, activation='relu'),
    Dense(32, activation='relu'),
    Dense(1)  # Output layer
])
```

## 📈 Results

- **Mean Absolute Error**: ~7-10 Lakhs
- **Training**: 100 epochs
- **Visualizations**: Actual vs Predicted prices, Feature correlations

## 💡 Usage Example

```python
# Manual prediction
Input: 1800 sqft, 3 bedrooms, 10 years, Delhi
Output: 🏠 Predicted Price: 128.54 Lakhs
```

## 📁 Files

- `House_Price_Prediction.ipynb` - Main notebook
- `house_prices.csv` - Dataset
- `requirements.txt` - Dependencies

## 👨‍💻 Author

Aravind R Nair

---

*Simple and effective house price prediction using deep learning*
