I have been analyzing exhange data to build a prediction model for data mining course.

Currently I am in the feature generation step.


## Data

Data contains following columns:
- NO-record number
- SECCODE-instrument code
- BUYSELL-buy/sell(B/S)
- TIME-timestamp HHMMSSZZZXXX format
- ORDERNO-order number; what exactly considered as order?
- ACTION-type of order 0-revoke, 1-post, 2-match
- PRICE-price of the order
- VOLUME-the volume of the order
- TRADENO-trade number
- TRADEPRICE-price of the deal

There are rougly 6 million row in each file. There are about 27 files in each folder. There are three folders for three months.


## This repository contains:
- notebook to create orderbook for each trading day. Code with Pandas and Cython processes each day in about 9 seconds
- notebook to create features like:
  - orderbook spectrum
  - volume weighted average(VWAP)
  - volumes of trades(aggressors)
  - liquidity replenishment
  - bid-ask spread
  
  
  
  I am open to suggestions and comments.
