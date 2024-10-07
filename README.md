# CryptoChronicles - Advanced Forecasting and Analysis of Bitcoin Price Movements

**Aim**: The aim of this project is to leverage advanced machine learning techniques and time-series forecasting methods to analyze and predict Bitcoin price movements. It also seeks to identify trends, anomalies, and volatility patterns to enhance decision-making in cryptocurrency markets.

## Libraries Used
- `pandas`
- `numpy`
- `datetime`, `timedelta`
- `yfinance`
- `mplfinance`
- `matplotlib`, `seaborn` (for visualizations)
- `statsmodels` (for ARIMA/SARIMA models)
- `prophet` (for time series forecasting)
- `tensorflow`, `keras` (for LSTM models)
- `scikit-learn` (for clustering with Dynamic Time Warping)
- `arch` (for GARCH volatility modeling)
- `stable-baselines3` (for reinforcement learning)

## Methodologies

### 1. Data Collection
- Collected 10 years of Bitcoin data from Yahoo Finance using the `yfinance` library.

### 2. Data Preprocessing
   - Data cleaning, handling missing values, and normalizing.
   - Feature engineering to create relevant variables for time series forecasting.

### 3. Time Series Forecasting
   - Implemented ARIMA and SARIMA models to forecast future Bitcoin prices.
   - Optimized ARIMA parameters using grid search.
   - Used the Prophet model to capture seasonality and holiday effects.
   - Built an LSTM network to predict future Bitcoin price trends.

### 4. Clustering Analysis
   - Used Dynamic Time Warping (DTW) to measure similarity between different time periods of Bitcoin's price movement.
   - Performed clustering to identify similar patterns like bull and bear markets.

### 5. Volatility Modeling
   - Applied GARCH models to estimate and forecast the volatility in Bitcoin prices over time.

### 6. Reinforcement Learning for Trading
   - Developed an RL agent using Deep Q-Networks (DQN) to make buy/sell decisions.
   - Trained the agent on historical Bitcoin data to maximize profit based on reward signals.

## Visualization Techniques

- **Line Plots**: Visualized the time series data of Bitcoin prices to observe trends over time.
- **Candlestick Charts**: Used `mplfinance` to create candlestick charts for a clearer representation of price fluctuations in specific periods.
- **Correlation Heatmaps**: Utilized `seaborn` to generate heatmaps that displayed the correlation between different financial indicators.
- **Moving Averages**: Overlaid moving averages on price data to highlight trends and support trading decisions.
- **Volatility Plots**: Created volatility graphs using GARCH model outputs to illustrate the fluctuation intensity of Bitcoin prices.
- **Anomaly Detection Visualizations**: Highlighted detected anomalies from the Prophet model on top of the original time series data.

## Insights
- **ARIMA/SARIMA** models provided reasonably accurate forecasts, with seasonality playing a role during specific periods.
- **Prophet Model** captured weekly trends and helped to identify anomalies and holiday-related price movements.
- **LSTM Networks** showed potential for longer-term forecasting but required extensive tuning for optimal performance.
- **Clustering with DTW** revealed distinct time periods of similar price behaviors, highlighting the transitions between bull and bear markets.
- **GARCH Models** indicated significant volatility in Bitcoin prices, with notable spikes during high-market events.
- **Reinforcement Learning Agent** made profitable trades during high volatility periods, but performance varied based on the reward structure.
