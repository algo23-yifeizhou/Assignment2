# Assignment 2

### What is it about?
This project is a reproduce of 
  Baltussen, Da, Z., Lammers, S., & Martens, M. (2021). Hedging demand and market intraday momentum. Journal of Financial Economics, 142(1), 377–403. https://doi.org/10.1016/j.jfineco.2021.04.029

### Abstract
Hedging short gamma exposure requires trading in the direction of price movements, thereby creating price momentum. Using intraday returns on over 60 futures on equities, bonds, commodities, and currencies between 1974 and 2020, they find strong market intraday momentum everywhere. The return during the last 30 minutes before the market close is positively predicted by the return during the rest of the day (from previous market close to the last 30 minutes). The predictive power is economically and statistically highly significant, and reverts over the next days. We provide novel evidence that links market intraday momentum to the gamma hedging demand from market participants such as market makers of options and leveraged ETFs.
### My contribution and improvement
I reproduced the models in this paper, using Shanghai Stock 50 Index Exchange Traded Fund and its corresponding Exchange options, as there is no leveraged ETFs in Chinese Exchanges. 
### Conclusions
1. The phenomenon of Gamma pressure leading to the close momentum was not significant in China's SS50 ETF and its corresponding option markets. 
image.png
The picture above shows that the number of "NGE<0" observations is extremely small(41 observations/1476), compared with the Whole sample(1434 observations/1476). The following picture shows the OLS Regression Results of the "NGE>0" observations, both the t-statistics are significant, in other words, the NGE factor CAN NOT tell whether there would be a close momentum in SS50 ETF market.
image.png

Backtest of intraday momentum under "NGE<0" and "NGE>0" circumstances:
##### NGE<0
image.png
##### NGE>0
image.png

2. For one reason, the under developed derivative market in China might be to blame for this phenomenon. And on the other hand, one of the factors leading the close momentum referred in this paper does not make sense for all markets.

### Discussion

Though the NGE can hardly explain the intraday momentum in China's market, but what we have is that the momentum still exist, and what we need to do next is to find a better explanation for this phenomenon! 
