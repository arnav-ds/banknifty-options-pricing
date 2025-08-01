# BANKNIFTY Options Pricing Engine

This project implements a full-featured options pricing engine to analyze and model European call options on the BANKNIFTY index using real data from the National Stock Exchange of India (NSE).

The engine computes theoretical option prices using two widely used financial models: the Black-Scholes-Merton formula and the Binomial Tree model. It also calculates the full set of option Greeks and compares theoretical prices to actual market prices.

## Project Features

- Load and clean contract-wise BANKNIFTY options data
- Estimate historical volatility from spot price returns
- Compute time to expiry and risk-free rate inputs
- Price European call options using:
  - Black-Scholes-Merton closed-form model
  - Recombining Binomial Tree (Cox-Ross-Rubinstein method)
- Calculate Greeks: Delta, Gamma, Vega, Theta, Rho
- Analyze pricing error between theoretical and market prices
- Generate visualizations for price comparison and sensitivity

## Data

- Source: National Stock Exchange of India (www.nseindia.com)
- Dataset: Contract-wise Price Volume Data
- Underlying: BANKNIFTY Index Options (Call Options Only)
- Time Range: July–August 2025
- Format: CSV

## Technology Stack

- Python (Jupyter Notebook)
- pandas, numpy, scipy, matplotlib, seaborn
- No use of external pricing libraries; all pricing logic implemented from scratch

## Visual Outputs

- Market vs. Model Price comparison scatter plot
- Absolute pricing error vs. strike price
- Delta vs. Strike for a given expiry
- Combined price comparison: Black-Scholes, Binomial, Market

## Usage

1. Clone this repository:
git clone https://github.com/arnav-ds/banknifty-options-pricing.git
cd banknifty-options-pricing

2. Open the Jupyter Notebook:

jupyter notebook options_pricing_engine.ipynb

3. Run all cells to compute prices, Greeks, and visualizations.

4. Final results are exported as a CSV: `banknifty_options_pricing_results.csv`

## About European Call Options

A European call option is a financial contract that gives the holder the right, but not the obligation, to buy the underlying asset at a specified strike price, only on the option's expiration date. These options differ from American options in that they cannot be exercised before expiry. They are commonly used in index option markets, including BANKNIFTY.

## Author

**Arnav Anant**  
Data Science Undergraduate  
Savitribai Phule Pune University  
Email: anantarnav21@gmail.com  
LinkedIn: [https://www.linkedin.com/in/arnav-anant-4a1841342](https://www.linkedin.com/in/arnav-anant-4a1841342)  
GitHub: [https://github.com/arnav-ds](https://github.com/arnav-ds)

## License

This project is open-source and available under the MIT License.


