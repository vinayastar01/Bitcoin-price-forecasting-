# 🚀 Bitcoin Price Forecasting with TensorFlow

![📈 Bitcoin Price Prediction Example]

Time series forecasting project using deep learning to predict Bitcoin prices (2013–2021). Implements and compares multiple model architectures including Dense networks, CNN, and LSTM.

![download (2)](https://github.com/user-attachments/assets/e61fbf53-641b-4ceb-9328-11e277987c28)
![download3](https://github.com/user-attachments/assets/54c532a1-9657-42c5-a1e7-a8b487812e81)


## 🗂 Table of Contents
- [📌 Project Overview](#project-overview)
- [✨ Key Features](#key-features)
- [⚙️ Usage](#usage)
- [📊 Results](#results)
- [📁 File Structure](#file-structure)
- [📝 License](#license)

## 📌 Project Overview
This project implements and compares different deep learning architectures for time series forecasting of Bitcoin prices. The dataset contains daily Bitcoin prices from October 2013 to May 2021.

**🧠 Models Implemented:**
1. 🧮 Naive Baseline
2. 🏗 Dense Network (7-day window)
3. 🏗 Dense Network (30-day window)
4. 📏 Conv1D
5. 🔁 LSTM

**📈 Key Findings:**
- ✅ Simple Dense models outperformed more complex architectures
- 🥇 Best model: Dense network with 7-day window (MAE: $565.28)
- ❌ CNN and LSTM models underperformed in this implementation
- 📅 7-day window size works better than 30-day window

## ✨ Key Features
- 🧪 Multiple model architectures compared
- 🧩 Custom time series windowing implementation
- 💾 Model checkpointing and saving
- 📊 Visualization utilities
- 📐 Performance metrics comparison

```

## ⚙️ Usage

### 🏋️‍♂️ Training Models
```bash
python src/train.py
```

### 📊 Generate Visualizations
```bash
python src/visualize.py
```

### 📓 Run Jupyter Notebook
```bash
jupyter lab notebooks/Bitcoin_Price_Forecasting.ipynb
```

## 📊 Results

### 📏 Model Performance Comparison

| Model             | MAE     | MSE         | RMSE   |
|------------------|---------|-------------|--------|
| Naive Baseline   | 567.98  | 1,147,547   | 1,071  |
| Dense (7-day)    | 565.28  | 1,152,412   | 1,073  |
| Dense (30-day)   | 614.02  | 1,274,133   | 1,128  |
| Conv1D           | 17,166  | 519,000,000 | 22,785 |
| LSTM             | 20,017  | 707,000,000 | 26,606 |

### 🖼 Prediction Visualization
![Model Predictions](results/prediction_examples.png)

## 📁 File Structure

```
bitcoin-forecasting/
├── data/
│   └── BTC_USD_2013-10-01_2021-05-18-CoinDesk.csv
├── models/
│   ├── model_1_dense.keras
│   ├── model_2_dense.keras
│   ├── model_3_conv1D.keras
│   └── model_4_LSTM.keras
└── README.md
```

## 📝 License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

**📬 Contact:** [edu.vinay123@gmail.com]
