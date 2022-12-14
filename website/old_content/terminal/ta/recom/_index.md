```
usage: recom [-s {crypto,forex,cfd}] [-e EXCHANGE] [-i {1M,1W,1d,4h,1h,15m,5m,1m}] [--export {csv,json,xlsx}] [-h]
```

Print tradingview recommendation based on technical indicators. [Source: <https://pypi.org/project/tradingview-ta/>]

```
optional arguments:
  -s {crypto,forex,cfd}, --screener {crypto,forex,cfd}
                        Screener. See https://python-tradingview-ta.readthedocs.io/en/latest/usage.html (default: america)
  -e EXCHANGE, --exchange EXCHANGE
                        Set exchange. For Forex use: 'FX_IDC', and for crypto use 'TVC'. See https://python-tradingview-
                        ta.readthedocs.io/en/latest/usage.html. By default Alpha Vantage tries to get this data from the ticker. (default: )
  -i {1M,1W,1d,4h,1h,15m,5m,1m}, --interval {1M,1W,1d,4h,1h,15m,5m,1m}
                        Interval, that corresponds to the recommendation given by tradingview based on technical indicators. See https://python-
                        tradingview-ta.readthedocs.io/en/latest/usage.html (default: )
  --export {csv,json,xlsx}
                        Export dataframe data to csv,json,xlsx file (default: )
  -h, --help            show this help message (default: False)
```

Example:

```
2022 Feb 16, 11:31 (๐ฆ) /stocks/ta/ $ recom
               Ticker Recommendation
โโโโโโโโโโโณโโโโโโโโโโโโโโโโโณโโโโโโณโโโโโโโณโโโโโโโโโโ
โ         โ RECOMMENDATION โ BUY โ SELL โ NEUTRAL โ
โกโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโฉ
โ 1 month โ BUY            โ 15  โ 2    โ 9       โ
โโโโโโโโโโโผโโโโโโโโโโโโโโโโโผโโโโโโผโโโโโโโผโโโโโโโโโโค
โ 1 week  โ BUY            โ 14  โ 2    โ 10      โ
โโโโโโโโโโโผโโโโโโโโโโโโโโโโโผโโโโโโผโโโโโโโผโโโโโโโโโโค
โ 1 day   โ SELL           โ 5   โ 13   โ 8       โ
โโโโโโโโโโโผโโโโโโโโโโโโโโโโโผโโโโโโผโโโโโโโผโโโโโโโโโโค
โ 4 hours โ SELL           โ 4   โ 14   โ 8       โ
โโโโโโโโโโโผโโโโโโโโโโโโโโโโโผโโโโโโผโโโโโโโผโโโโโโโโโโค
โ 1 hour  โ SELL           โ 4   โ 13   โ 9       โ
โโโโโโโโโโโผโโโโโโโโโโโโโโโโโผโโโโโโผโโโโโโโผโโโโโโโโโโค
โ 15 min  โ SELL           โ 3   โ 13   โ 10      โ
โโโโโโโโโโโผโโโโโโโโโโโโโโโโโผโโโโโโผโโโโโโโผโโโโโโโโโโค
โ 5 min   โ SELL           โ 5   โ 12   โ 9       โ
โโโโโโโโโโโผโโโโโโโโโโโโโโโโโผโโโโโโผโโโโโโโผโโโโโโโโโโค
โ 1 min   โ SELL           โ 6   โ 11   โ 9       โ
โโโโโโโโโโโดโโโโโโโโโโโโโโโโโดโโโโโโดโโโโโโโดโโโโโโโโโโ
```
