```
usage: coint [-ts {OPTIONS}] [-p] [-s SIGNIFICANT] [-h] [--export {csv,json,xlsx,png,jpg,pdf,svg}]
```

Show co-integration between timeseries.

Cointegration is a statistical property of a collection (X1, X2, ..., Xk) of time series variables. First, all of the series must be integrated of order d (see Order of integration). Next, if a linear combination of this collection is integrated of order less than d, then the collection is said to be co-integrated. Formally, if (X,Y,Z) are each integrated of order d, and there exist coefficients a,b,c such that aX + bY + cZ is integrated of order less than d, then X, Y, and Z are cointegrated. Cointegration has become an important property in contemporary time series analysis. Time series often have trendsβeither deterministic or stochastic. In an influential paper, Charles Nelson and Charles Plosser (1982) provided statistical evidence that many US macroeconomic time series (like GNP, wages, employment, etc.) have stochastic trends. [Source: Wikipedia]

```
optional arguments:
  -ts {OPTIONS}, --timeseries {OPTIONS}
                        The time series you wish to test co-integration on. Can hold multiple timeseries. (default: None)
  -p, --plot            Plot Z-Values (default: False)
  -s SIGNIFICANT, --significant SIGNIFICANT
                        Show only companies that have p-values lower than this percentage (default: 0)
  -h, --help            show this help message (default: False)
  --export {csv,json,xlsx,png,jpg,pdf,svg}
                        Export raw data into csv, json, xlsx and figure into png, jpg, pdf, svg (default: )
```

Example:

```
2022 Feb 24, 06:03 (π¦) /econometrics/ $ coint msft.adj_close,aapl.adj_close,tsla.adj_close,googl.adj_close -p
                                  Cointegration Tests
ββββββββββββββββββββββββββββββββββ³βββββββββββ³ββββββββ³ββββββββ³ββββββββββββββββ³ββββββββββ
β Pairs                          β Constant β Gamma β Alpha β Dickey-Fuller β P Value β
β‘ββββββββββββββββββββββββββββββββββββββββββββββββββββββββββββββββββββββββββββββββββββββ©
β adj_close-msft/adj_close-aapl  β 46.62    β 1.58  β 0.00  β -1.86         β 0.35    β
ββββββββββββββββββββββββββββββββββΌβββββββββββΌββββββββΌββββββββΌββββββββββββββββΌββββββββββ€
β adj_close-msft/adj_close-tsla  β 130.28   β 0.18  β -0.01 β -2.82         β 0.06    β
ββββββββββββββββββββββββββββββββββΌβββββββββββΌββββββββΌββββββββΌββββββββββββββββΌββββββββββ€
β adj_close-msft/adj_close-googl β 21.38    β 0.10  β -0.01 β -2.51         β 0.11    β
ββββββββββββββββββββββββββββββββββΌβββββββββββΌββββββββΌββββββββΌββββββββββββββββΌββββββββββ€
β adj_close-aapl/adj_close-tsla  β 53.92    β 0.11  β -0.01 β -2.94         β 0.04    β
ββββββββββββββββββββββββββββββββββΌβββββββββββΌββββββββΌββββββββΌββββββββββββββββΌββββββββββ€
β adj_close-aapl/adj_close-googl β -7.83    β 0.06  β -0.00 β -1.62         β 0.47    β
ββββββββββββββββββββββββββββββββββΌβββββββββββΌββββββββΌββββββββΌββββββββββββββββΌββββββββββ€
β adj_close-tsla/adj_close-googl β -505.14  β 0.51  β -0.01 β -2.28         β 0.18    β
ββββββββββββββββββββββββββββββββββ΄βββββββββββ΄ββββββββ΄ββββββββ΄ββββββββββββββββ΄ββββββββββ
```

![error_terms_cointegrations](https://user-images.githubusercontent.com/46355364/155514964-dd75cf17-91ae-4326-96e8-45d9a2c7b24a.png)
