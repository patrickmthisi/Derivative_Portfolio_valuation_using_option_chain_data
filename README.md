# Derivative_Portfolio_valuation_using_option_chain_data
# Project description and objectives:

This study involves the market-based valuation of a portfolio of non-traded American options on the Tesla (TSLA) stock. The option chain data used in the end-to-end project was sourced from Yahoo Finance.  

The main highlights of this project involve:
1. Calibrating our model to market quotes of liquidly traded options.
2. The model used for simulation was a jump-diffusion model, given by:

$$S_{t_{m+1}} = \Big(exp\Big(\Big(r - r_j - \frac{\sigma^2}{2}\Big)(t_{m+1} - t_{m}) + \sigma\sqrt{t_{m+1} - t_{m}}z_{t}^{1}\Big) + \Big(exp(\mu_{j} + \sigma z_{t}^{2}) - 1\Big)y_t\Big) \\n 0 \le t_m \le t_{m+1} \le T$$

3. Using the calibrated model for the pricing of a portfolio of non-traded American put options using Least Squares Monte Carlo.
4. Calculating the overall portfolio value, as well as risk metrics such as delta and vega.
