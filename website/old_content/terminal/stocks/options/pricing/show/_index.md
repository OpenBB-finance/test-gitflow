```
usage: show [-h]
```

Shows the list of prices and probabilities entered using the add command.

```
optional arguments:
  -h, --help            show this help message (default: False)
```

Example:

```
2022 Feb 16, 09:45 (๐ฆ) /stocks/options/pricing/ $ add -p 100 -c 0.5

2022 Feb 16, 09:46 (๐ฆ) /stocks/options/pricing/ $ add -p 200 -c 0.5

2022 Feb 16, 09:46 (๐ฆ) /stocks/options/pricing/ $ show
Estimated price(s) of AAPL at 2022-05-20
โโโโโโโโโโณโโโโโโโโโ
โ Price  โ Chance โ
โกโโโโโโโโโโโโโโโโโโฉ
โ 100.00 โ 0.50   โ
โโโโโโโโโโผโโโโโโโโโค
โ 200.00 โ 0.50   โ
โโโโโโโโโโดโโโโโโโโโ
```
