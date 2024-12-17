#Question 1

import yfinance as yf
import pandas as pd
import matplotlib.pyplot as plt

data = yf.download("AAPL", period="1y")
closing_prices = data[['Close']]
print(closing_prices)

plt.figure(figsize=(16, 10)) 
plt.plot(closing_prices.index, closing_prices['Close'], label='AAPL Close Price', color='b')

plt.title("AAPL Closing Prices For 2024")
plt.xlabel("Date")
plt.ylabel("Closing Price in USD")

plt.show()

#Apple Inc.(AAPL) stock has been experiencing an upward trend over the past year with massive fluctuations in between. Despite a few brief drops, the general trend remains positive, showing strong growth for the company.
