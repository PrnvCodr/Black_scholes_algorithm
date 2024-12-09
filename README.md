# Black-Scholes Option Pricing Model

This repository implements the **Black-Scholes** model for pricing European call and put options. The Black-Scholes formula is a widely used mathematical model that allows for the calculation of theoretical option prices based on various parameters such as the underlying asset's price, strike price, time to maturity, volatility, and the risk-free interest rate.

## Features
- **European Option Pricing**: Calculates both call and put option prices using the Black-Scholes formula.
- **Greeks Calculation**: Computes key "Greeks" (Delta and Gamma) to measure option price sensitivity.
- **Visualization**: Includes interactive graphs and visualizations of option prices across different asset prices and volatilities.
- **Customization**: Easily modify key parameters like strike price, volatility, and time to maturity to see how they affect option pricing.
- **Additional Models**: Optional extensions to other models (e.g., Binomial Model) for more complex option pricing scenarios.

## Parameters
- **Current Asset Price**: The current price of the underlying asset.
- **Strike Price**: The price at which the option can be exercised.
- **Time to Maturity**: The time remaining until the option expires (in years).
- **Volatility (σ)**: The standard deviation of the asset's returns, representing price fluctuation.
- **Risk-Free Interest Rate**: The theoretical interest rate for an investment with no risk of loss.
- **Number of Steps** (for Binomial Model): The number of steps to use in the binomial tree model.

## How to Use

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/black-scholes-model.git
   cd black-scholes-model
