🚀 Stock Price Prediction – AAPL (Apple Inc.)

This project is part of the Data Science Internship at Arch Technologies. The goal is to predict the **future closing stock prices** of Apple Inc. (AAPL) using historical stock data. Two different models are used for performance comparison:

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

🗓️ Time Range: January 1, 2020 – January 1, 2025

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

### 🔹 Data Collection & Cleaning

- Downloaded 5 years of AAPL stock data using `yfinance`
- Removed missing values
- Focused on features: `Open`, `High`, `Low`, `Volume` → Predicting `Close`

### 🔹 Exploratory Data Analysis (EDA)

- Correlation heatmap  
- Line plots for price trends  
- Residual plot for error analysis  

### 🔹 Feature Engineering

- Time-based train-test split (80/20)
- Sequence creation for LSTM (60-day sliding window)
- Scaling features using MinMaxScaler for LSTM

---

🧠 Model Training

### 📘 Model 1: Linear Regression

- Used Scikit-learn's `LinearRegression`
- Trained on selected features
- Evaluation Metrics:
  - MSE, RMSE, MAE, R² Score
- Visualizations:
  - Actual vs Predicted Plot
  - Residual Distribution Plot

### 📗 Model 2: LSTM Neural Network

- Built using TensorFlow / Keras
- Two LSTM layers + Dense output layer
- Trained on sequential, scaled data
- Evaluation Metrics:
  - MSE, RMSE, MAE
- Visualizations:
  - Actual vs Predicted Trend Plot

---

📈 Model Performance

| Metric       | Linear Regression | LSTM Model |
|--------------|------------------:|-----------:|
| MAE          | 📉 Moderate        | ✅ Lower   |
| RMSE         | 📉 Higher          | ✅ Lower   |
| R² Score     | 📉 Basic Fit       | ✅ Stronger Fit |
| Visual Match | ❌ Random mismatch | ✅ Trend aligned |

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
