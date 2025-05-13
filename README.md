# Reliance Stock Prices Prediction Using LSTM

Predict the future prices of Reliance Industries stock using a deep learning LSTM model trained on historical data from Yahoo Finance.

[Read the full walkthrough on Medium &rarr;](https://reddykarthikeya1.medium.com/reliance-stock-prices-prediction-using-lstm-a-full-walkthrough-ad1c06bd00a0)

---

## 📈 Project Overview

This project demonstrates how to build and evaluate a Long Short-Term Memory (LSTM) neural network to forecast Reliance Industries' stock prices. The workflow includes:

- Downloading historical stock data using `yfinance`
- Feature engineering (moving averages, returns, etc.)
- Data scaling and sequence creation for LSTM input
- Model building and training with TensorFlow/Keras
- Evaluation and visualization of predictions
- Multi-step (7-day) future forecasting

---

## 🗂️ Repository Structure

```
best_lstm_model.h5                # Trained LSTM model weights
model.ipynb                       # Main Jupyter notebook (full code & analysis)
tf_gpu/                           # Python virtual environment (TensorFlow GPU)
```

---

## 🚀 Quick Start

1. **Clone the repository**
   ```sh
   git clone https://github.com/yourusername/reliance-stock-lstm.git
   cd reliance-stock-lstm
   ```

2. **Set up the environment**
   - (Recommended) Use the provided `tf_gpu/` virtual environment, or create your own:
     ```sh
     python -m venv tf_gpu
     source tf_gpu/Scripts/activate  # On Windows
     # or
     source tf_gpu/bin/activate      # On Linux/Mac
     pip install -r requirements.txt
     ```

3. **Run the notebook**
   - Open `model.ipynb` in Jupyter or VS Code and run all cells.

---

## 📊 Example Results

![LSTM Predictions vs Actual](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*QvQnQkQKpQnQkQKpQnQkQ.png)

*Above: Actual vs. Predicted closing prices on the test set.*

---

## 🧠 Model Highlights

- **Architecture:** 2 LSTM layers with dropout and L2 regularization, followed by dense layers.
- **Features:** Close price, volume, 50/200-day moving averages, daily returns.
- **Evaluation:** RMSE and MAE metrics, plus visual comparison.
- **Forecasting:** Supports single-step and 7-day multi-step predictions.

---

## 📚 Learn More

For a detailed explanation, code walkthrough, and insights, check out the [Medium article](https://reddykarthikeya1.medium.com/reliance-stock-prices-prediction-using-lstm-a-full-walkthrough-ad1c06bd00a0).

---

## 🛠️ Dependencies

- Python 3.7+
- yfinance
- pandas, numpy, matplotlib
- scikit-learn
- tensorflow (with GPU support recommended)

Install all dependencies with:
```sh
pip install -r requirements.txt
```

---

## 📄 License

This project is for educational and research purposes only. Refer to Yahoo's [terms of use](https://policies.yahoo.com/us/en/yahoo/terms/index.htm) for data usage.

---

## 🙏 Acknowledgements

- [Yahoo Finance](https://finance.yahoo.com/) for data
- [TensorFlow](https://www.tensorflow.org/) for deep learning
- [Keras](https://keras.io/) for model building

---

> *Inspired by [reddykarthikeya1's Medium article](https://reddykarthikeya1.medium.com/reliance-stock-prices-prediction-using-lstm-a-full-walkthrough-ad1c06bd00a0).*
