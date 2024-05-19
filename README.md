# Dividend-Policy-Predictor-x-New-Horizons-Financial
## About Project
Creating models predicts dividend changes for the upcoming year. These models will enable users to input a stock ticker and receive a forecast of how the dividends for that stock are expected to change over the next year. By leveraging these models, our clients can make more informed investment decisions and better manage their portfolios. The primary goal is to provide accurate and actionable insights into future dividend trends, enhancing the financial planning and strategy development for our clients.
## Introduction
### Objective of the project  
- Develop predictive models that provide forecasts of dividend changes for the next year based on inputted stock tickers.  
### Importance of the project  
- Enabling informed investment decisions
- Optimizing portfolio management
### Business Impact  
- Enhancing the ability to anticipate and respond to market changes
- Improving risk management and economic forecasting  
## Project structure
![Project Architect Diagram](https://github.com/bw24ca/Dividend-Policy-Predictor-x-New-Horizons-Financial/blob/main/Project%20Architect%20Diagram.png)
## Data Source
### What is the dataset?
Financial Data for S&P 500 Stocks (2013-2022)
### Where we retrieved the data (Sources)？
Collected through API calls from three sources:  
#### FMP(Financial Modeling Prep)  
- Gather financial data such as dividend, different ratios, company earnings, etc.  
#### FRED(Federal Reserve Bank of St.Louis)
- Gather information such as inflation rates, interest rates, etc.  
#### Yahoo Finance  
- Stock ticker, company’s industry & sector  
### Important features    
- A total of 180 features included in our dataset, ex.Adjusted Dividend, company ratings, interest rate, inflation, etc  
## Data Processing and Dataset Selection
### Data Processing
To develop predictive models for forecasting dividend changes, we focused on processing the financial data to create meaningful datasets. The processing steps included:  

1.Creating Three Distinct Datasets:
- Dataset 1: Excluded stocks with 0 dividend throughout the entire 10-year period.
- Dataset 2: Excluded stocks with 5 consecutive years without dividend payouts (i.e., stocks with 0 dividend from 2019 to 2023).
- Dataset 3: The original dataset, including all stocks in the S&P 500.
  
2.Handling Missing Values:  
- Filled NA values with 0 in all datasets.
- Removed stocks with missing financial ratios or data from financial statements, as these are unlikely to be NA or zero.

### Dataset Selection  
After evaluating the datasets, we chose Dataset 2 for the following reasons:

- **Relevance to Client Needs:** This dataset focuses on stocks with dividend payouts, which aligns with our client's goal of predicting dividend cuts. By using stocks that have a history of dividend payouts, we can train the models more effectively to provide accurate forecasts.  
- **Data Quality:** Removing stocks with extended periods of zero dividends ensures the dataset is representative of stocks that are actively paying dividends, enhancing the model's predictive power.
  
By selecting Dataset 2, we ensure our predictive models are trained on relevant and high-quality data, thus providing the best results for forecasting dividend changes. 




