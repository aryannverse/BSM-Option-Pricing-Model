
<h1 align="center" style="font-weight: bold;">BSM Option Pricing Model 💵</h1>


<p align="center">A web-based interactive tool for pricing European call and put options using the Black-Scholes-Merton (BSM) model. This project allows users to input option parameters, visualize results, and analyze sensitivities through heatmaps and charts. It is built for finance professionals, students, and anyone interested in quantitative finance.</p>


<p align="center">
<a href="https://bsm-aryannverse.streamlit.app/">Visit the project!</a>
</p>

<h2>Preview: </h2>
<img width="1689" alt="Screenshot 2025-07-03 at 4 38 28 PM" src="https://github.com/user-attachments/assets/82e9d3fd-3593-4a32-b18a-4a1998916340" />

<h2>What is the Black-Scholes-Merton (BSM) model?</h2>
The Black-Scholes-Merton (BSM) model is a mathematical model used to calculate the theoretical price of European-style options. Developed by Fischer Black, Myron Scholes, and Robert Merton, it revolutionized financial markets by providing a closed-form solution for option pricing.

<h3>Core Concepts:<h3>

<b>Purpose:<b> Computes fair prices for European call and put options, helping traders and investors make informed decisions.

<b>Inputs:<b>

- Current price of the underlying asset

- Strike price of the option

- Time to maturity (in years)

- Volatility of the underlying asset (annualized standard deviation)

- Risk-free interest rate (annualized, continuous compounding)

- Outputs: The model provides the theoretical price for both call and put options, as well as sensitivities like delta and gamma.

<h3>Mathematical Formulation:<h3>


The model uses the following formulas:

<img width="317" alt="96b07712-aa53-4e2c-ae2f-2931e1fec7ab" src="https://github.com/user-attachments/assets/7a3c431f-2e6f-41a4-ac74-7cc69db316b5" />

 
Where:

S: Current price of the underlying asset

K: Strike price

T: Time to maturity (years)

r: Risk-free interest rate

σ: Volatility

Call Option Price:
<img width="318" alt="Screenshot 2025-07-03 at 4 59 57 PM" src="https://github.com/user-attachments/assets/72e64ba9-a4bc-41ee-b4b5-a6c1d560474f" />


Put Option Price:
<img width="348" alt="Screenshot 2025-07-03 at 5 00 03 PM" src="https://github.com/user-attachments/assets/2683a4d7-b32b-4b5e-b3c4-3962f8ff59c3" />

Where: 

<b> N(x)<b> is the cumulative distribution function of the standard normal distribution.

Assumptions:

The underlying asset follows a geometric Brownian motion with constant volatility and drift.

No dividends are paid during the life of the option.

Markets are frictionless (no transaction costs or taxes).

The risk-free rate and volatility are constant.

The option can only be exercised at expiration (European style).

Practical Use:

- The BSM model is widely used in financial markets for pricing, risk management, and strategy development.
- It also provides "Greeks" (sensitivities) like delta and gamma, which are crucial for hedging and risk assessment


<h2 id="technologies">💻 Technologies</h2>

- Streamlit (web application framework)
- NumPy (numerical computations)
- Pandas (data manipulation)
- SciPy (statistical functions, e.g., normal CDF)
- Matplotlib (data visualization)
- Seaborn (statistical data visualization)
- Plotly (interactive plots)



<h2>Cloning</h2>

How to clone the project to run it locally: 

```bash
git clone https://github.com/aryannverse/BSM-Option-Pricing-Model
```

<h2>Prerequisites</h2>

Prerequisite necessary for running your project. 

- `yfinance`: To fetch current asset prices.


<h2>Starting</h2>

Here's how to start the project:

```bash
cd BSM-Option-Pricing-Model
pip install -r requirements.txt
streamlit run 'app.py'
```
