```
usage: tipt [-l LIMIT] [-h] [--export {csv,json,xlsx}]
```

Print top insider purchases of the day. [Source: OpenInsider]

```
optional arguments:
  -l LIMIT, --limit LIMIT
                        Limit of datarows to display (default: 10)
  -h, --help            show this help message (default: False)
  --export {csv,json,xlsx}
                        Export raw data into csv, json, xlsx (default: )
```

Example:

```
2022 Feb 16, 08:18 (๐ฆ) /stocks/ins/ $ tipt
                                                                          Insider Data
โโโโโณโโโโโโโโโโโโโโณโโโโโโโโโโโโโณโโโโโโโโโณโโโโโโโโโโโโโโโโโโโณโโโโโโโโโโโโโโโโโโโโโโโณโโโโโโโโโโโณโโโโโโโโโโโโโโโณโโโโโโโโณโโโโโโโโโโณโโโโโโโโโโณโโโโโโโโโโโณโโโโโโโโโโโโ
โ X โ Filing Date โ Trade Date โ Ticker โ Company Name     โ Insider Name         โ Title    โ Trade Type   โ Price โ Qty     โ Owned   โ Diff Own โ Value     โ
โกโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโฉ
โ M โ 2022-02-16  โ 2022-02-09 โ ZIVO   โ Zivo Bioscience, โ Maggiore Christopher โ Dir, 10% โ P - Purchase โ $3.72 โ +91,334 โ 803,105 โ +13%     โ +$340,098 โ
โ   โ 06:02:09    โ            โ        โ Inc.             โ D.                   โ          โ              โ       โ         โ         โ          โ           โ
โโโโโดโโโโโโโโโโโโโโดโโโโโโโโโโโโโดโโโโโโโโโดโโโโโโโโโโโโโโโโโโโดโโโโโโโโโโโโโโโโโโโโโโโดโโโโโโโโโโโดโโโโโโโโโโโโโโโดโโโโโโโโดโโโโโโโโโโดโโโโโโโโโโดโโโโโโโโโโโดโโโโโโโโโโโโ
M: Multiple transactions in filing; earliest reported transaction date & weighted average transaction price
```
