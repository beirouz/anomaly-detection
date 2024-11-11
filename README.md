# Anomaly Detection in Financial Data

This repository contains code and documentation related to using statistical and machine learning techniques to enhance anomaly detection in financial data. The project focuses on detecting data quality issues by analyzing stock prices from several financial institutions over a specified period.

## Project Overview

### Problem Statement
In financial services, accurate calculation of risk statistics and other metrics relies heavily on input data quality. A sudden increase or drop in input data values can significantly impact output data and lead to low-quality data products. Therefore, capturing and treating anomalies in input data is essential to ensure consistent historical output data. This project explores various statistical and machine learning approaches to identify the best anomaly detection methods for different use cases.

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

### Key Insights
- **Machine Learning Models**: ML-based models offer the advantage of reusability across multiple data products, allowing for faster anomaly detection without repeated data analysis. However, these models often act as "black boxes," making it difficult to fully explain their behavior and results. Communicating the reasons for anomalies to data providers can be challenging and requires careful adjustment of detection thresholds, often through trial and error.
- **Statistical Methods**: Statistical methods, while more transparent and easier to justify in terms of threshold adjustment, may not generalize well across different use cases. For instance, Z-score methods may perform poorly on datasets with heavy tails, while other methods may work better for specific distributions.

## Usage

### Installation
To install the necessary dependencies:
```bash
pip install -r requirements.txt
