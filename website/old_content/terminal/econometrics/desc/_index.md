```
usage: desc [-n {OPTIONS}] [-h] [--export {csv,json,xlsx}]
```

Show the descriptive statistics of a dataset.

```
optional arguments:
  -n {OPTIONS}, --name {OPTIONS}
                        The name of the database you want to show the descriptive statistics for (default: None)
  -h, --help            show this help message (default: False)
  --export {csv,json,xlsx}
                        Export raw data into csv, json, xlsx (default: )
```

Example:
```
2022 Jun 01, 06:50 (๐ฆ) /econometrics/ $ load anes96

2022 Jun 01, 06:51 (๐ฆ) /econometrics/ $ desc anes96

                                       Statistics for dataset: 'anes96'                                        
โโโโโโโโโณโโโโโโโโโโณโโโโโโโโโณโโโโโโโโโณโโโโโโโโโณโโโโโโโโโณโโโโโโโโโณโโโโโโโโโณโโโโโโโโโณโโโโโโโโโณโโโโโโโโโณโโโโโโโโโโโ
โ       โ popul   โ tvnews โ selflr โ clinlr โ dolelr โ pid    โ age    โ educ   โ income โ vote   โ logpopul โ
โกโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโฉ
โ count โ 944.00  โ 944.00 โ 944.00 โ 944.00 โ 944.00 โ 944.00 โ 944.00 โ 944.00 โ 944.00 โ 944.00 โ 944.00   โ
โโโโโโโโโผโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโผโโโโโโโโโผโโโโโโโโโผโโโโโโโโโผโโโโโโโโโผโโโโโโโโโผโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโค
โ mean  โ 306.38  โ 3.73   โ 4.33   โ 2.94   โ 5.39   โ 2.84   โ 47.04  โ 4.57   โ 16.33  โ 0.42   โ 2.47     โ
โโโโโโโโโผโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโผโโโโโโโโโผโโโโโโโโโผโโโโโโโโโผโโโโโโโโโผโโโโโโโโโผโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโค
โ std   โ 1082.61 โ 2.68   โ 1.44   โ 1.38   โ 1.27   โ 2.27   โ 16.42  โ 1.60   โ 5.97   โ 0.49   โ 3.19     โ
โโโโโโโโโผโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโผโโโโโโโโโผโโโโโโโโโผโโโโโโโโโผโโโโโโโโโผโโโโโโโโโผโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโค
โ min   โ 0.00    โ 0.00   โ 1.00   โ 1.00   โ 1.00   โ 0.00   โ 19.00  โ 1.00   โ 1.00   โ 0.00   โ -2.30    โ
โโโโโโโโโผโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโผโโโโโโโโโผโโโโโโโโโผโโโโโโโโโผโโโโโโโโโผโโโโโโโโโผโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโค
โ 25%   โ 1.00    โ 1.00   โ 3.00   โ 2.00   โ 5.00   โ 1.00   โ 34.00  โ 3.00   โ 14.00  โ 0.00   โ 0.10     โ
โโโโโโโโโผโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโผโโโโโโโโโผโโโโโโโโโผโโโโโโโโโผโโโโโโโโโผโโโโโโโโโผโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโค
โ 50%   โ 22.00   โ 3.00   โ 4.00   โ 3.00   โ 6.00   โ 2.00   โ 44.00  โ 4.00   โ 17.00  โ 0.00   โ 3.10     โ
โโโโโโโโโผโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโผโโโโโโโโโผโโโโโโโโโผโโโโโโโโโผโโโโโโโโโผโโโโโโโโโผโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโค
โ 75%   โ 110.00  โ 7.00   โ 6.00   โ 4.00   โ 6.00   โ 5.00   โ 58.00  โ 6.00   โ 21.00  โ 1.00   โ 4.70     โ
โโโโโโโโโผโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโผโโโโโโโโโผโโโโโโโโโผโโโโโโโโโผโโโโโโโโโผโโโโโโโโโผโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโค
โ max   โ 7300.00 โ 7.00   โ 7.00   โ 7.00   โ 7.00   โ 6.00   โ 91.00  โ 7.00   โ 24.00  โ 1.00   โ 8.90     โ
โโโโโโโโโดโโโโโโโโโโดโโโโโโโโโดโโโโโโโโโดโโโโโโโโโดโโโโโโโโโดโโโโโโโโโดโโโโโโโโโดโโโโโโโโโดโโโโโโโโโดโโโโโโโโโดโโโโโโโโโโโ

2022 Jun 01, 06:51 (๐ฆ) /econometrics/ $ desc anes96.educ

Statistics for dataset: 'anes96'
โโโโโโโโโณโโโโโโโโโ
โ       โ educ   โ
โกโโโโโโโโโโโโโโโโโฉ
โ count โ 944.00 โ
โโโโโโโโโผโโโโโโโโโค
โ mean  โ 4.57   โ
โโโโโโโโโผโโโโโโโโโค
โ std   โ 1.60   โ
โโโโโโโโโผโโโโโโโโโค
โ min   โ 1.00   โ
โโโโโโโโโผโโโโโโโโโค
โ 25%   โ 3.00   โ
โโโโโโโโโผโโโโโโโโโค
โ 50%   โ 4.00   โ
โโโโโโโโโผโโโโโโโโโค
โ 75%   โ 6.00   โ
โโโโโโโโโผโโโโโโโโโค
โ max   โ 7.00   โ
โโโโโโโโโดโโโโโโโโโ
```
