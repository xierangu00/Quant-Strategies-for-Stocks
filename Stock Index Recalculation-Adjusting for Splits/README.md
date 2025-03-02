# Detailed Stock Index Analysis

## Overview

This project is designed to provide a detailed analysis of the components of a stock index, specifically focusing on the impact of stock splits on the index calculation. The aim is to adjust stock prices for splits, recalculate the index, and understand how these adjustments affect the overall index value.

## Project Objectives

- To calculate the number of shares for each stock within an index based on its market value.
- To adjust stock prices to account for stock splits and ensure accurate market representation.
- To recalculate the stock index using adjusted prices and compare the adjusted index with the pre-adjustment values.
- To update the divisor used in the index calculation post-adjustments for continuous accuracy.

## Dependencies

This project requires Python and the installation of the yfinance package, which allows for the fetching of real-time and historical market data from Yahoo Finance.

### Required Software and Libraries

- Python 3.x
- yfinance

## Installation Guide

To set up the project environment, follow these steps:

```bash
# Install Python and pip if not already installed
# Install yfinance using pip
pip install yfinance
```

## Usage Instructions

* **Data Fetching**: Use the yfinance library to fetch historical data for stocks listed in the index.
* Calculations:
  * Calculate the number of shares for each stock by dividing the total dollar value of the index by the price of each stock.
  * Adjust stock prices in the event of a split to maintain consistency in market value representation.
* Analysis:
  * Compare the original and adjusted stock prices
  * Recalculate the index values using both the original and adjusted prices.
  * Calculate the new divisor necessary for the index post-adjustment.

## Detailed Code Explanation

* Share Calculation:
  * Code calculates how many shares of each stock are present in the index based on the index's dollar value and individual stock prices.
* Adjusting for Stock Splits:
  * Adjust stock prices for splits by modifying the stock price directly in the dataset. This step ensures that the analysis reflects real-world conditions where stock splits have occurred.
* Display Adjusted Prices:
  * Output the adjusted prices to verify correctness.
* Index Recalculation:
  * Use adjusted prices along with the original divisor to recalculate the index value. This shows the impact of the stock split.
* New Divisor Calculation:
  * Determine a new divisor based on the adjusted prices, which is crucial for maintaining the accuracy of the index moving forward.

## Conclusion

This project helps in understanding the dynamics of stock indices in response to market changes such as stock splits. By maintaining an accurate calculation of index values, stakeholders can make informed decisions based on precise market data.
