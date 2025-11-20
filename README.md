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

- Employee A – score: X
- Employee B – score: Y
- Employee C – score: Z

### Top 3 Negative Employees (latest month)

- Employee D – score: P
- Employee E – score: Q
- Employee F – score: R

*(You can get these from `rankings_df` for the latest `year_month`.)*

### Flight-Risk Employees

Employees who sent ≥4 negative emails in any rolling 30-day period:

- Employee X
- Employee Y
- Employee Z

*(List from `flight_risk_unique`.)*

## 4. Insights & Recommendations

- Overall sentiment is mostly Neutral with some pockets of sustained negativity.
- Certain months show lower average sentiment, possibly linked to specific events.
- Frequent negative senders should be monitored and engaged by HR / management.
- The regression model indicates that message frequency and negative message count are important drivers of the monthly sentiment score.
