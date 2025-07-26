📈 Stock Price Prediction – AAPL (Apple Inc.)

This project is part of the Data Science Internship at Arch Technologies. The goal is to predict the **future closing stock prices** of Apple Inc. (AAPL) using historical stock data. Two different models are used for comparison:

- ✅ Linear Regression (Classical Machine Learning)
- 🔁 LSTM (Long Short-Term Memory – Deep Learning)

---

📁 Dataset

The dataset is downloaded using the `yfinance` Python library and includes:

- Open
- High
- Low
- Close (Target)
- Volume  
- Time range: **January 1, 2020 – January 1, 2025**

---

📊 Technologies Used

- Python 🐍  
- Jupyter Notebook  
- yfinance  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn  
- TensorFlow / Keras  

---

✅ Project Steps

### 📊 Data Collection & Cleaning
- Downloaded 5 years of AAPL stock data using `yfinance`
- Removed missing values
- Focused on relevant features: `Open`, `High`, `Low`, `Volume` to predict `Close`

---

### 🧠 Feature Engineering & EDA
- Time-based train-test split (80/20)
- Correlation heatmap
- Line plots for trend analysis
- Residual analysis (for Linear Regression)

---

### ⚙️ Model Training

#### Model 1: Linear Regression
- Used Scikit-learn's `LinearRegression`
- Trained on time-sorted data
- Evaluated using:
  - MSE, RMSE, MAE, R² Score
- Plotted **Actual vs Predicted** Closing Prices
- Residual plot for error distribution

#### Model 2: LSTM (Deep Learning)
- Used TensorFlow/Keras to build a 2-layer LSTM model
- Scaled data using `MinMaxScaler`
- Created 60-day input sequences
- Evaluated using:
  - MSE, RMSE, MAE
- Plotted **Actual vs Predicted** using time-series aligned data

---

📈 Model Performance

| Metric       | Linear Regression | LSTM Model |
|--------------|------------------:|-----------:|
| MAE          | ✔️ Lower          | ✅ Lower   |
| RMSE         | ✔️ Moderate       | ✅ Better  |
| R² Score     | 📉 Basic Fit      | ✅ Good Fit |
| Visual Match | 📉 Line mismatch (random split) | ✅ Trend match |

---

📂 Files in this Repo

| File                     | Description                                |
|--------------------------|--------------------------------------------|
| `Stock_Prediction.ipynb` | Main notebook with both models             |
| `README.md`              | Project summary and model explanation      |
| `AAPL_data.csv` (optional) | Raw downloaded data (if saved)             |

---

✍️ Author

**Ayesha Nadeem**  
Data Science Intern – July 2025  
Arch Technologies  

---

📧 Contact

For technical issues or feedback:  
📩 **ayeshanadeem2408@gmail.com**
