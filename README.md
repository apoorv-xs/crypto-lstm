# 🧠 Coinseer: Cryptocurrency Price Prediction with LSTM

Coinseer is a deep learning project that predicts cryptocurrency closing prices using Long Short-Term Memory (LSTM) networks. It processes time-series data from multiple coins (like Bitcoin, Ethereum, Litecoin, and Dogecoin) with lag-based feature engineering to forecast future price movements.

---

## 📊 Features

- Loads historical price data for multiple coins from Google Drive
- Automatically generates lag features
- Scales data using MinMaxScaler
- Reshapes features for LSTM input
- Trains and evaluates LSTM models per coin and for a combined dataset
- Visualizes actual vs predicted prices
- Computes and displays Mean Squared Error (MSE)

---

## 🚀 Technologies Used

- Python 3
- Pandas, NumPy
- Scikit-learn
- TensorFlow / Keras
- Matplotlib
- Google Colab

---

## 📂 Project Structure

```
coinseer/
├── aithing_dogecoin.ipynb        # Dogecoin prediction notebook
├── coin_combined_lstm.ipynb      # (Optional) Multi-coin combined model
├── data/
│   └── coin_Bitcoin.csv          # Add your CSVs here
│   └── coin_Dogecoin.csv
├── README.md
├── requirements.txt
└── .gitignore
```

---

## 📥 Data Format

Your `.csv` files should be named like:  
```
coin_Bitcoin.csv
coin_Ethereum.csv
coin_Dogecoin.csv
```

Each file should have at least the following columns:
```
Date, Open, High, Low, Close, Volume
```

Place them in:  
```
/content/drive/MyDrive/Coin/
```

---

## 📈 How to Use

1. Upload your `.csv` coin files to Google Drive:  
   `MyDrive/Coin/coin_<CoinName>.csv`

2. Open the notebook (`crypto.ipynb`) in Google Colab

3. Run the cells:
   - Data preprocessing
   - Feature creation
   - LSTM training
   - Prediction + Plotting

4. View prediction plots and MSE score

---

## 🧪 Example Output

| Coin      | MSE         |
|-----------|-------------|
| Dogecoin  | 0.00017     |
| Bitcoin   | 0.00012     |
| Ethereum  | 0.00020     |

(With corresponding prediction plots shown in the notebook)

---

## 📦 Installation (Optional Local Setup)

```bash
pip install -r requirements.txt
```

### requirements.txt
```
pandas
scikit-learn
tensorflow
matplotlib
```

---

## 🛡️ License

MIT License. See `LICENSE` file for details.

---

## 👤 Author

Made with ❤️ by Apoorv A S  
> Predict responsibly. Crypto is volatile 😄
