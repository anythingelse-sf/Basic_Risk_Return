## Background

Evalute four investment options on key risk-management metrics:\
The daily retuns\
Standard deviations\
Sharpe ratio\
beta\

Import the CSV file to create a single DataFrame and do a risk analysis of the assets vs the S&P 500. The evaluation should use rolling statistics to track the risk-reward behavior over time.

## Instructions
# Prepare your data
1) Import the data
2) Set the DateTimeIndex
3) Use the Pandas pct_change function together with dropna to create daily returns for this index

# Analyze by performance
1) Find the daily returns for each fund\
2) Plot the daily returns\
3) Find the cumulative returns for each fund\
4) Plot the cumulative returns

Returns: The S&P 500 is the best performer.

# Analyze by Volatility
1) Use the Pandas plot function with a box parameter
2) Drop out the S&P and run the box plots again

Returns: The most volatile is Berkshire Hathaway, the least volatile being Tiger Global Management.

# Analyze by Risk [using Standard Deviation]
1) Review the standard deviations
2) Sort smallest to largest
3) Find the annualized standard deviation (std * sqrt of 252 days)
4) Plot the standard deviation for 21 day rolling periods
5) Cut out the S&P500 to run again, comparing only the funds

Which of the four portfolios offers the best risk-return profile? Which offers the worst?
I'm taking Berkshire and Tiger. Tiger has the least volatility and has peformed ok. Berkshire has more volatility but it also has the most return.

# Diversify the portfolio and run it again

Use the pd.var function to calculate the variance of the S&P 500 by using a 60-day rolling window. Visualize the last five rows of the variance of the S&P 500.

Choose two portfolios that you chose, complete the following steps:

1) Using a 60-day window, calculate the covariance for each fund.
2) Using a 60-day window, calculate the beta for each fund
3) Plot each value


# Analysis

Answer the following questions:

Do any of the four fund portfolios outperform the S&P 500 index? 
- No, the S&P is the best performer based on the cumprod() function.

Based on the box plot visualization of just the four fund portfolios, which fund was the most volatile (with the greatest spread) and which was the least volatile (with the smallest spread)?
- Berkshire Hathaway is the most volatile of the four funds. Tiger Global is the least volatile. 

Based on the annualized standard deviation, which portfolios pose more risk than the S&P 500?
- None of the funds have a wider annualized standard deviation than the S&P 500

Based on the rolling metrics, does the risk of each portfolio increase at the same time that the risk of the S&P 500 increases?
- The funds seem to be mainly uncorrelated to the S&P 500 until 2020 happens. All of the rolling standard deviation of returns rise during the beginning of 2020.

Based on the rolling standard deviations of only the four fund portfolios, which portfolio poses the most risk? Does this change over time?
- Berkshire has the highest risk overall, but Paulson has been rising in the last two years. Should of invested with Paulson in 2008 and went home.

Which of the four portfolios offers the best risk-return profile? Which offers the worst? 
- Berkshire Hathaway has the best Sharpe Ratio. It actually is better than that of the S&P 500, although the S&P 500 has a better overall return during this time period. 

# Select two portfolios to continue the analysis
Which of the two portfolios seem more sensitive to movements in the S&P 500?
- Berkshire Hathaway is more sensitve to the movements in the S&P 500

Which of the two portfolios do you recommend for inclusion in your firm’s suite of fund offerings?
- Tiger Global, it has a lower beta over the rolling windows and also a lower covaraince. It will be a more useful fund to protect against the downside of the S&P 500.

Additional Comments:
- An interesting tidbit is that the Sharpe Ratio for Berkkshire is higher than that of the S&P 500. It may be useful to invest in a portfolio using the Berkshire Hathaway and the Tiger Global funds and dropping the index. 

