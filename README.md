# Employee-Sentiment-Analysis

## 1. Project Overview

This project analyzes internal employee emails to:
- Automatically label each message with sentiment (Positive, Negative, Neutral)
- Perform Exploratory Data Analysis (EDA)
- Compute monthly sentiment scores per employee
- Rank employees based on sentiment
- Identify potential flight-risk employees
- Build a linear regression model to analyze/predict sentiment trends

## 2. How to Run

1. Place `test.csv` in the project root.
2. Open `Employee_Sentiment_Analysis.ipynb` in Jupyter Notebook.
3. Run all cells in order.
4. Outputs will be saved in:
   - `outputs/` (CSV summaries)
   - `visualizations/` (plots in PNG format)

## 3. Key Results

### Top 3 Positive Employees (latest month)

- kayne.coulter@enron.com – score: 14
- eric.bass@enron.com  – score: 9
- lydia.delgado@enron.com  – score: 9

### Top 3 Negative Employees (latest month)

- bobette.riner@ipgdirect.com – score: 1
- rhonda.denton@enron.com  – score: 1
- sally.beck@enron.com  – score: 2

### Flight-Risk Employees

Employees who sent ≥4 negative emails in any rolling 30-day period:

- eric.bass@enron.com
- johnny.palmer@enron.com
- patti.thompson@enron.com
- sally.beck@enron.com


## 4. Insights & Recommendations

- Overall sentiment is mostly Neutral with some pockets of sustained negativity.
- Certain months show lower average sentiment, possibly linked to specific events.
- Frequent negative senders should be monitored and engaged by HR / management.
- The regression model indicates that message frequency and negative message count are important drivers of the monthly sentiment score.
