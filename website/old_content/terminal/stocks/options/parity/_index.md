```
usage: parity [-p] [-a] [-m MINI] [-M MAXI] [-h] [--export {csv,json,xlsx}]
```

An advanced strategy that seeks arbitrage opportunites in put-call spreads relative to the forward underlying asset price; put-call parity defines the relationship between calls, puts and the underlying futures contract. This principle requires that the puts and calls are the same strike, same expiration and have the same underlying futures contract.  The put call relationship is highly correlated, so if put call parity is violated, an arbitrage opportunity exists.

```
optional arguments:
  -p, --put             Shows puts instead of calls (default: False)
  -a, --ask             Use ask price instead of lastPrice (default: False)
  -m MINI, --min MINI   Minimum strike price shown (default: None)
  -M MAXI, --max MAXI   Maximum strike price shown (default: None)
  -h, --help            show this help message (default: False)
  --export {csv,json,xlsx}
                        Export raw data into csv, json, xlsx (default: )
```

Example:

```
2022 Feb 16, 09:17 (๐ฆ) /stocks/options/ $ load TSLA

2022 Feb 16, 09:18 (๐ฆ) /stocks/options/ $ parity -m 900 -M 950
Warning: Low volume options may be difficult to trade.
โโโโโโโโโโณโโโโโโโโโโโโโโโโโโ
โ Strike โ Call Difference โ
โกโโโโโโโโโโโโโโโโโโโโโโโโโโโฉ
โ 900.00 โ -3.49           โ
โโโโโโโโโโผโโโโโโโโโโโโโโโโโโค
โ 905.00 โ -3.37           โ
โโโโโโโโโโผโโโโโโโโโโโโโโโโโโค
โ 910.00 โ -4.09           โ
โโโโโโโโโโผโโโโโโโโโโโโโโโโโโค
โ 915.00 โ -1.39           โ
โโโโโโโโโโผโโโโโโโโโโโโโโโโโโค
โ 920.00 โ -2.34           โ
โโโโโโโโโโผโโโโโโโโโโโโโโโโโโค
โ 925.00 โ -2.65           โ
โโโโโโโโโโผโโโโโโโโโโโโโโโโโโค
โ 930.00 โ -2.46           โ
โโโโโโโโโโผโโโโโโโโโโโโโโโโโโค
โ 935.00 โ -5.14           โ
โโโโโโโโโโผโโโโโโโโโโโโโโโโโโค
โ 940.00 โ -3.89           โ
โโโโโโโโโโผโโโโโโโโโโโโโโโโโโค
โ 945.00 โ -8.08           โ
โโโโโโโโโโผโโโโโโโโโโโโโโโโโโค
โ 950.00 โ -3.23           โ
โโโโโโโโโโดโโโโโโโโโโโโโโโโโโ
```
