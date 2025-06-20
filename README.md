# Close Price Forecasting using ARIMA, Prophet, and Stacked LSTM
  This project explores and compares three approaches to forecast stock market closing prices:

1. ARIMA – Traditional statistical method
2. Facebook Prophet – Seasonality-aware forecasting
3. Stacked LSTM – Deep learning model for sequential prediction

**Stacked LSTM outperformed** both ARIMA and Prophet in prediction accuracy and trend capture.

**Objective:-**
To forecast future close prices of a stock (e.g., yahoo) using historical data and analyze:

  1. Accuracy of each model  
  2. Ability to capture short and long-term patterns
  3. Suitability for real-world financial forecasting

**Dataset**

• **Source**: Yahoo Finance (yahoo.csv)  
• **Target Column**: Close  
• **Duration**: ~5 years of daily data  
• **Preprocessing**:  
      • Missing values handled   
      • MinMax scaling (for LSTM)  
      • Date parsing  

**Tools & Libraries used:-**

    • pandas, numpy
    • statsmodels (ARIMA)
    • prophet by Facebook
    • tensorflow, keras (LSTM)
    • matplotlib

**Models Overview**

**1. ARIMA**  
  • Classical autoregressive model  
  • Best for short-term, linear trends  
  • Limited handling of seasonality/nonlinearity  

**2️. Facebook Prophet**  
  • Captures trend, seasonality, and holiday effects    
  • Great for irregular time series and robust to missing dates  
  • Interpretable and quick to deploy  

**3️. Stacked LSTM (Best Model)**  
  • Multiple LSTM layers stacked to learn complex temporal dependencies  
  • Handles non-linear patterns, volatility, and long-term memory  
  • Outperformed others in capturing reversals and fine-grained trends  

**Visualizations**  
  • Forecast vs Actual (All Models) Plots    
  • Prophet Trend & Seasonality Plots  

**Results Summary**

  • In ARIMA, I got almost straight line ; which was seemed to be a mean line ; did'nt got good results!!  
  • In Prophet , I got a similar curve but not that much steeper as expected !!  
  • Stacked LSTM generalized better and captured complex patterns in stock price movements.
  
