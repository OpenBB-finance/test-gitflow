```
usage: add [-p PRICE] [-c CHANCE] [-h]
```

Add price and probability points to the list

```
optional arguments:
  -p PRICE, --price PRICE
                        Projected price of the stock at the expiration date (default: None)
  -c CHANCE, --chance CHANCE
                        Chance that the stock is at a given projected price (default: None)
  -h, --help            show this help message (default: False)
```

Example:

```
2022 Feb 16, 09:42 (๐ฆ) /stocks/options/pricing/ $ add -p 175 -c 0.5

2022 Feb 16, 09:43 (๐ฆ) /stocks/options/pricing/ $ add -p 165 -c 0.5

2022 Feb 16, 09:43 (๐ฆ) /stocks/options/pricing/ $ show
Estimated price(s) of AAPL at 2022-05-20
โโโโโโโโโโณโโโโโโโโโ
โ Price  โ Chance โ
โกโโโโโโโโโโโโโโโโโโฉ
โ 165.00 โ 0.50   โ
โโโโโโโโโโผโโโโโโโโโค
โ 175.00 โ 0.50   โ
โโโโโโโโโโดโโโโโโโโโ
```
