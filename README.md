# Time Series Project - Stock Price
- This project was developed for **forecasting Samsung Electronics' Stock Price**.

## Data Processing
- Handling Missing Values: Same value, Interpolation → make two datasets
- Detecting and managing outliers: IQR, Winsorizing, Z-score, Quantile Clipping
- Standardization & Logarithm Transform: Applied differently depending on the feature
- 1st Differencing
- Additional steps: One-Hot Encoding, Decomposing, Correlation, PCA      
➡️ Fully processed Data with 43 features


## Modeling
- Baseline: Smoothing (SES, DES, Holt-Winters)
- ARIMAX, SARIMAX
- XGBoost: Grid Search
- LSTM: Random Search
- Transformer: Grid Search

## Experiments
We conducted Experiments only with LSTM and Transformer because other models showed poor performance. 
- Before Outlier Detection + Feature Selection
- Before Outlier Detection + Scaling + Feature Selection 
- Fully Processed Data + Feature selection    
➡️ Best was **3rd option with LSTM model**


## Prior Knowledge
We added prior knowledge, that is **Stock Split**, to the best model.
It showed the best performance.