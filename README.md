# 📉 Bitcoin Strategy: Golden Cross & Crash Detection

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Library](https://img.shields.io/badge/Library-Scikit--Learn-orange)
![Strategy](https://img.shields.io/badge/Strategy-Golden--Cross-gold)
![Status](https://img.shields.io/badge/Status-Completed-success)

## 📌 Project Overview
This project applies Machine Learning and Technical Analysis to Bitcoin (BTC) historical data to identify trading opportunities and detect potential market crashes. 

The core strategy revolves around the **"Golden Cross"** (a bullish signal) and uses a **Random Forest Classifier** to predict market movements based on key technical indicators.

**Author:** Muhammad Atif

## 📂 Dataset
The project analyzes historical Bitcoin market data.
- **Data Source:** Likely Kaggle or Yahoo Finance (BTC-USD).
- **Key Features:** `Open`, `High`, `Low`, `Close`, `Volume`.
- **Derived Features:**
  - **SMA (Simple Moving Average):** Calculated for short-term (e.g., 50-day) and long-term (e.g., 200-day) trends.
  - **RSI (Relative Strength Index):** To measure overbought or oversold conditions.

## 🛠 Tech Stack
- **Language:** Python
- **Data Analysis:** `pandas`, `numpy`
- **Visualization:** `matplotlib`, `seaborn`
- **Machine Learning:** `scikit-learn` (Random Forest Classifier)

## 📊 Key Concepts Implemented

### 1. Golden Cross Strategy ⚱️
The code likely identifies moments where the **Short-Term SMA** crosses *above* the **Long-Term SMA**. This is traditionally seen as a major breakout signal.

### 2. Crash Detection 📉
By analyzing volatility and RSI spikes, the model attempts to flag periods where the market is overheating and prone to a sharp correction (crash).

## ⚙️ Project Workflow

### 1. Data Preprocessing
- Loaded historical BTC data.
- Cleaned missing values.
- Calculated Technical Indicators:
  - **SMA_50** & **SMA_200**
  - **RSI (14-day)**

### 2. Exploratory Data Analysis (EDA)
- Visualized Bitcoin price history.
- Plotted Moving Averages to visually identify Golden Cross events.
- Analyzed correlation between Volume and Volatility.

### 3. Model Training
- **Algorithm:** **Random Forest Classifier**.
- **Goal:** Classify the next market movement (e.g., Buy Signal vs. Sell/Crash Signal).
- **Split:** Data was split into Training and Testing sets to validate performance.

### 4. Evaluation
- **Confusion Matrix:** To see how many "Crashes" or "Rallies" were correctly predicted.
- **Feature Importance:** Identified which indicator (RSI vs. SMA) was most critical for the prediction.

## 🚀 How to Run

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/your-username/bitcoin-strategy.git](https://github.com/your-username/bitcoin-strategy.git)
