## Background

Evalute four investment options on key risk-management metrics:\
The daily retuns\
Standard deviations\
Sharpe ratio\
beta\

Import the CSV file to create a single DataFrame and do a risk analysis of the assets vs the S&P 500. The evaluation should use rolling statistics to track the risk-reward behavior over time.

## Instructions
# Prepare your data
1) Import the data\
2) Set the DateTimeIndex\
3) Use the Pandas pct_change function together with dropna to create daily returns for this index

# Analyze the performance
1)Find the daily returns for each fund\
2) Plot the daily returns\
3) Find the cumulative returns for each fund\
4) Plot the cumulative returns\

The S&P 500 is the best performer.

# Analyze the Volatility
1) Use the Pandas plot function with a box parameter\
2) Drop out the S&P and run the box plots again\

The most volatile is Berkshire Hathaway, the least volatile being-

# Analyze the Risk
1) Review the standard deviations\
2) Sort smallest to largest\
3) Find the annualized standard deviation (std * sqrt of 252 days)\
4) Plot the standard deviation for 21 day rolling periods\
5) Cut out the S&P500 to run again, comparing only the funds