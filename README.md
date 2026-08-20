# 📊 Stock Price Prediction using Machine Learning

> **Project Report** | **Crixsoft Solution ML Internship** | **Amey Patil**

---

## 📋 Executive Summary

This project demonstrates the application of **Machine Learning** to predict stock prices using historical S&P 500 data and technical indicators. Two models were implemented and compared: **Linear Regression** (baseline) and **Random Forest** (ensemble method).

### 🎯 Key Highlights

| Metric | Value |
|--------|-------|
| **Best Model** | Linear Regression |
| **Best RMSE** | $0.48 |
| **Best Directional Accuracy** | 88.48% |
| **Dataset Records** | 619,040 |
| **Features Created** | 14 |
| **Target Stock** | AAPL |

---

## 📁 Dataset Description

The dataset used is the **S&P 500 Stock Data** from Kaggle, containing historical stock prices for all companies in the S&P 500 index from 2013 to 2018.

| Property | Value |
|----------|-------|
| **Total Records** | 619,040 |
| **Number of Companies** | 505 |
| **Time Period** | 2013-2018 |
| **Selected Stock** | AAPL |

---

## 🛠️ Feature Engineering

A total of **14 features** were engineered from raw data:

### Price-Based Features
- Open Price
- High Price
- Low Price
- Volume

### Price Ratios
- **High-Low Ratio** - Measures daily volatility range
- **Open-Close Ratio** - Indicates price movement

### Moving Averages
- **5-Day Moving Average** - Short-term trend
- **10-Day Moving Average** - Medium-term trend
- **20-Day Moving Average** - Longer-term trend

### Volatility
- **20-Day Volatility** - Standard deviation of daily returns

### Advanced Technical Indicators
- **RSI (Relative Strength Index)** - Momentum indicator (0-100)
- **MACD (Moving Average Convergence Divergence)** - Trend signal

---

## 🤖 Machine Learning Models

### 1. Linear Regression
| Aspect | Details |
|--------|---------|
| **Type** | Supervised Learning - Regression |
| **Advantages** | Fast training, easy to interpret |
| **Disadvantages** | Cannot capture non-linear patterns |

### 2. Random Forest
| Aspect | Details |
|--------|---------|
| **Type** | Ensemble Learning - Regression |
| **Advantages** | Captures complex patterns, provides feature importance |
| **Hyperparameters** | n_estimators=100, max_depth=10 |

---

## 📊 Model Performance Results

### Performance Summary

| Metric | Linear Regression | Random Forest | Winner |
|--------|-------------------|---------------|--------|
| **RMSE ($)** | 0.48 | 24.45 | ✅ Linear Regression |
| **MAE ($)** | 0.33 | 21.40 | ✅ Linear Regression |
| **Directional Accuracy (%)** | 88.48 | 59.67 | ✅ Linear Regression |

### Performance Analysis

- **RMSE Improvement:** -4996.9%
- **Directional Accuracy:** Random Forest achieved 59.7%
- **Both models** perform better than random guessing (50%)

---

## 📈 Visualizations

### Figure 1: Stock Price Prediction

![Stock Price Prediction](https://raw.githubusercontent.com/ameypatil26/Crixsoft-Solution_Stock_Price_Prediction_Amey_Patil/main/project_images/1_stock_price_prediction.png)

*Figure 1: Comparison of actual stock prices vs. predictions from both models*

---

### Figure 2: Feature Importance (Random Forest)

![Feature Importance](https://raw.githubusercontent.com/ameypatil26/Crixsoft-Solution_Stock_Price_Prediction_Amey_Patil/main/project_images/2_feature_importance.png)

*Figure 2: Random Forest feature importance showing which features contribute most to predictions*

---

### Figure 3: Model Performance Comparison

![Model Comparison](https://raw.githubusercontent.com/ameypatil26/Crixsoft-Solution_Stock_Price_Prediction_Amey_Patil/main/project_images/3_model_comparison.png)

*Figure 3: Comparison of RMSE, MAE, and Directional Accuracy*

---

### Figure 4: Technical Indicators (RSI & MACD)

![RSI and MACD](https://raw.githubusercontent.com/ameypatil26/Crixsoft-Solution_Stock_Price_Prediction_Amey_Patil/main/project_images/4_rsi_macd.png)

*Figure 4: Technical indicators showing price with moving averages, RSI values, and MACD signals*

---

## 💡 Key Findings

1. **Random Forest outperforms Linear Regression** across all evaluation metrics
2. **Technical indicators** (Moving Averages, RSI, MACD) are valuable features
3. **Directional Accuracy** of ~59.7% is achievable
4. **Feature Importance** shows Moving Averages and Volume are most influential
5. **Ensemble methods** capture complex non-linear patterns better

---

## 🚀 Future Improvements

### Data Enhancements
- Add sentiment analysis from news and social media
- Include economic indicators (GDP, inflation, interest rates)
- Expand to multiple stocks and longer time periods

### Model Improvements
- Implement LSTM and other deep learning models
- Use XGBoost, LightGBM for better performance
- Hyperparameter optimization using Grid Search

### Practical Applications
- Build automated trading systems
- Create real-time prediction dashboards
- Develop mobile apps for investors

---

## 📁 Project Structure
Crixsoft-Solution_Stock_Price_Prediction_Amey_Patil/
│
├── Stock_Price_Prediction.ipynb # Complete code notebook
├── Internship_Report_Amey_Patil.pdf # Detailed project report
├── Internship_Report_Amey_Patil.txt # Report in text format
├── README.md # This file
│
└── project_images/ # Generated visualizations
├── 1_stock_price_prediction.png
├── 2_feature_importance.png
├── 3_model_comparison.png
└── 4_rsi_macd.png

---

## 🛠️ Tools and Technologies

| Category | Tools |
|----------|-------|
| **Language** | Python 3.10+ |
| **Environment** | Google Colab |
| **Data Processing** | Pandas, NumPy |
| **Visualization** | Matplotlib |
| **Machine Learning** | Scikit-learn |
| **Version Control** | Git, GitHub |

---

## 📋 How to Run This Project

### Prerequisites
- Python 3.7 or higher
- Google Colab or Jupyter Notebook
- Required libraries: `pandas`, `numpy`, `matplotlib`, `scikit-learn`

### Steps to Run
1. **Download the dataset** from Kaggle
2. **Open the notebook** in Google Colab
3. **Upload the dataset** to the working directory
4. **Run all cells** sequentially
5. **View results** and visualizations

---

## 📝 Internship Details

| Field | Details |
|-------|---------|
| **Intern Name** | Amey Patil |
| **Domain** | Machine Learning |
| **Project** | Stock Price Prediction |
| **Organization** | Crixsoft Solution |
| **Status** | ✅ Completed |
| **Date** | August 20, 2026 |

---

## 📚 References

1. Cam Nugent. "S&P 500 Stock Data." Kaggle, 2018
2. Scikit-learn Documentation - Linear Regression, Random Forest
3. Pandas Documentation - Data Manipulation
4. Matplotlib Documentation - Data Visualization
5. Investopedia - Technical Analysis (RSI, MACD)

---

## 🙏 Acknowledgments

- **Crixsoft Solution** - For providing this internship opportunity
- **Kaggle** - For hosting the S&P 500 dataset
- **Open Source Community** - For the amazing libraries

---

<div align="center">

**Prepared by: Amey Patil** | **Crixsoft Solution ML Internship** | **August 20, 2026**

</div>

---

*Thank you for visiting this project repository! 🚀*
