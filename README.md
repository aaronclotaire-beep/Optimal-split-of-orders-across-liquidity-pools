# Optimal-split-of-orders-across-liquidity-pools
We implement the stochastic approximation algorithm described on page 11 for the optimal allocation of buy orders in dark pools under a shortage configuration.  
That is, the total volume available in the dark pools is smaller than the volume we want to execute, so the remaining volume is executed on the regular market.

We generate pseudo-realistic data following the approach proposed on page 15, based on order book data from certain stocks on the Paris Stock Exchange.  

> **Note:** For proprietary reasons, the original data used in the study is not included.  
> Each dataset is represented as a `DataFrame` containing all transactions with the same format:

* `Time` (index): timestamp of the transaction  
* `TradedPrice`: average price per share in the transaction  
* `TradedQty`: volume of the transaction  

This structure allows you to run the notebooks and reproduce the stochastic approximation algorithm using synthetic or similar datasets.
