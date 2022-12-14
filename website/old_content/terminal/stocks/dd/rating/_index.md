```
usage: rating [-l LIMIT] [-h] [--export {csv,json,xlsx}]
```

Based on specific ratios, prints information whether the company is a (strong) buy, neutral or a (strong) sell. The following fields are expected: P/B, ROA, DCF, P/E, ROE, and D/E. [Source: Financial Modeling Prep]

```
optional arguments:
  -l LIMIT, --limit LIMIT
                        limit of last days to display ratings
  -h, --help            show this help message
  --export {csv,json,xlsx}
                        Export raw data into csv, json, xls
```

Example (Google):

```
2022 Feb 16, 04:34 (๐ฆ) /stocks/dd/ $ rating
                                           Rating
โโโโโโโโโโโโโโณโโโโโโโโโณโโโโโโโโโโโโโณโโโโโโโโโโณโโโโโโโโโโณโโโโโโโโโโณโโโโโโโโโโโโโณโโโโโโโโโโโโโ
โ            โ Rating โ DCF        โ ROE     โ ROA     โ DE      โ PE         โ PB         โ
โกโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโฉ
โ 2022-02-15 โ Buy    โ Strong Buy โ Neutral โ Neutral โ Neutral โ Strong Buy โ Strong Buy โ
โโโโโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโโโโโค
โ 2022-02-14 โ Buy    โ Strong Buy โ Neutral โ Neutral โ Neutral โ Strong Buy โ Strong Buy โ
โโโโโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโโโโโค
โ 2022-02-11 โ Buy    โ Strong Buy โ Neutral โ Neutral โ Neutral โ Strong Buy โ Strong Buy โ
โโโโโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโโโโโค
โ 2022-02-10 โ Buy    โ Strong Buy โ Neutral โ Neutral โ Neutral โ Strong Buy โ Strong Buy โ
โโโโโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโโโโโค
โ 2022-02-09 โ Buy    โ Strong Buy โ Neutral โ Neutral โ Neutral โ Strong Buy โ Strong Buy โ
โโโโโโโโโโโโโโดโโโโโโโโโดโโโโโโโโโโโโโดโโโโโโโโโโดโโโโโโโโโโดโโโโโโโโโโดโโโโโโโโโโโโโดโโโโโโโโโโโโโ
```
