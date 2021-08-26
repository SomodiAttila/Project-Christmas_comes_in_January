# Project---Christmas-comes-in-January
A time series analysis project that examines the January Effect seasonal anomaly of international stock markets.

## Goal of the project
The goal of this project is to find **investment oppurtunities** by taking advantage of the seasonal stock market anomaly, the January Effect.
This study wants to answer the following questions:
1. Is the January Effect present at the chosen stock markets?
2. Is there a difference between **small, medium and large companies** regarding the anomaly?
3. Is there a pattern we can see between the different **countries**?

## The January Effect
The January Effect is the perceived seasonal tendency for **stocks to rise** in that month.
Like other market anomalies and calendar effects, the January Effect is considered by some to be evidence against the efficient markets hypothesis.

The cause behind the January Effect is attributed to tax-loss harvesting, consumer sentiment, year-end bonuses, raising year-end report performances, and more.

The January Effect appears to affect **small-cap stocks more than large-cap** stocks.

## Data
I collected data from MSCI's website. I formatted the data in Excel. You can access it in the repository.

I collected data from **15 MSCI stock indices**. Collected data for small, medium and large companies from all chosen markets, so **in total I had 45 time series**.

## Approach
My approach was to use statistical techniques to find out how returns behave in each month (not just in January) for each of the chosen markets.

First I transformed the time series data into **log returns**, so I could get **stationary** time series. 
I looked at the log return plots, the ACF and PACF plots, the descriptive statistics and the ADF values to decide to use an **OLS regression model with dummy variables** for each month. I also used Newey-West standard errors for autocorrelation and heteroskedasticity.

## Results

![image](https://user-images.githubusercontent.com/89580600/130972755-f0338f4a-4de1-43e2-a233-efaa25901b66.png)

1. I can reject the presence of January Effect based on the evidence of the regression model.
2. April and December showed to be significant in all 3 capitalization categories.
3. Some markets were more efficient than others but April and December produced significant positive returns on average for many countries.
