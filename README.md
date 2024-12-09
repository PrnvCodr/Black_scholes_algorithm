# Black-Scholes Option Pricing Model

This repository implements the **Black-Scholes Option Pricing Model** to compute the theoretical prices of European call and put options. The Black-Scholes model uses a continuous-time framework for pricing options and is widely used in finance for its analytical formula.

## 🚀 Features
- https://black-scholes-algorithm.streamlit.app/
- **Option Pricing**: Computes prices for European call and put options.
- **Greeks Calculation**: Calculates option sensitivities, including Delta and Gamma.
- **Interactive Heatmaps**: Explore how option prices change with spot prices and volatility using Streamlit.
- **Python-Based Implementation**: A straightforward, extensible Python implementation for learning and professional use.

---

## 📋 Parameters
| Parameter               | Description                                       |
|-------------------------|---------------------------------------------------|
| `current_price`         | Price of the underlying asset.                    |
| `strike`                | Strike price of the option.                       |
| `time_to_maturity`      | Time to maturity (in years).                      |
| `volatility`            | Annualized volatility of the underlying asset.    |
| `interest_rate`         | Risk-free interest rate (annualized).             |

---

## 🛠 Installation
1. Clone this repository:
    ```bash
    git clone https://github.com/your-username/black-scholes-option-pricing.git
    ```
2. Navigate to the project directory:
    ```bash
    cd black-scholes-option-pricing
    ```
3. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

---

## 📝 Usage
### Basic Example
```python
from black_scholes import BlackScholes

# Initialize parameters
time_to_maturity = 2  # in years
strike = 90           # strike price
current_price = 100   # current asset price
volatility = 0.2      # annualized volatility
interest_rate = 0.05  # annualized risk-free interest rate

# Instantiate the model
model = BlackScholes(
    time_to_maturity=time_to_maturity,
    strike=strike,
    current_price=current_price,
    volatility=volatility,
    interest_rate=interest_rate
)

# Calculate prices
call_price, put_price = model.calculate_prices()

# Print results
print(f"Call Option Price: {call_price}")
print(f"Put Option Price: {put_price}")
print(f"Call Delta: {model.call_delta}")
print(f"Put Delta: {model.put_delta}")
print(f"Call Gamma: {model.call_gamma}")
print(f"Put Gamma: {model.put_gamma}")
