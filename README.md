# Anomaly Detection in Financial Data

This repository contains code and documentation related to using statistical and machine learning techniques to enhance anomaly detection in financial data. The project focuses on detecting data quality issues by analyzing stock prices from several financial institutions over a specified period.

## Project Overview

### Problem Statement
In financial services, accurate calculation of risk statistics and other metrics relies heavily on input data quality. The project explores the use of statistical and modern machine learning approaches for effective anomaly detection.

### Data Sources
The `yfinance` library was used to retrieve adjusted closing prices for the following institutions:
- JPMorgan Chase & Co. (JPM)
- Goldman Sachs Group Inc. (GS)
- Morgan Stanley (MS)
- BlackRock Inc. (BLK)
- Citigroup Inc. (C)

### Key Components
1. **Data Preprocessing and Visualization**: Summary statistics, pair plots, and Q-Q plots are used to provide insights into data distribution and relationships.
2. **Anomaly Detection Methods**:
   - **Statistical Approaches**:
     - Interquartile Range (IQR) method
     - Rolling Median and Median Absolute Deviation (MAD)
     - Mahalanobis Distance
   - **Machine Learning Techniques**:
     - Vector Autoregression (VAR)
     - Kalman Filter
     - K-Nearest Neighbors (KNN)
     - Isolation Forest
     - Autoencoder (Dense and LSTM-based models)

3. **Results and Findings**: The models identified anomalies in time series data, providing insights into rare but significant deviations from expected patterns.

## Usage

### Installation
To install the necessary dependencies:
```bash
pip install -r requirements.txt
