# CNN-Based Stock Price Forecasting

## Project Overview
This project explores the use of **Convolutional Neural Networks (CNNs)** to predict stock price movements by transforming historical stock data into **candlestick chart images**. Inspired by Jiang, Kelly, and Xiu (2021), the approach challenges traditional numerical models by leveraging image-based pattern recognition.

## Problem Statement
Stock market prediction is complex due to volatile and non-linear data. Traditional models rely on historical prices but fail to generalize well. This project investigates whether **image-based deep learning models** can outperform these traditional methods.

## Data
- **Source**: Yahoo Finance & CRSP Database
- **Variables**: Open, High, Low, Close, Volume (OHLCV)
- **Period**: 1993-2019

## Methodology
1. **Image Conversion**:  
   - Convert OHLC data into candlestick chart images.
   - Add moving averages (5, 20, 60-day).
2. **Model Architecture**:  
   - CNN with convolutional, pooling, batch normalization, and fully connected layers.
   - Three models based on different input timeframes: 5-day, 20-day, 60-day.
3. **Training**:  
   - Loss: Cross-Entropy  
   - Optimizer: Adam (learning rate: 1e-5)  
   - Regularization: Dropout (50%), Batch Normalization

## Results
- **Accuracy**: CNN models outperformed traditional momentum and reversal strategies.
- **Sharpe Ratio**: CNN portfolio achieved a Sharpe Ratio up to **2.71**, surpassing conventional benchmarks.
- **Interpretability**: Saliency maps and logistic regression provided insights into CNN decision-making.

## Limitations
- Computationally expensive.
- Interpretability remains a challenge.

## Future Work
- Use Grad-CAM for better interpretability.
- Experiment with CNN-RNN hybrids.
- Extend to crypto, forex, and global markets.

## Contributors
- Ananth Mohan
- Dhairya Dedhia
