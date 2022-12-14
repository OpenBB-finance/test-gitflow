```
usage: var [-m] [-a] [-s] [-p PERCENTILE] [-h]
```

Provides value at risk (short: VaR) of the selected stock.

```
optional arguments:
  -m, --mean            If one should use the mean of the stocks return (default: False)
  -a, --adjusted        If the VaR should be adjusted for skew and kurtosis (Cornish-Fisher-Expansion) (default:
                        False)
  -s, --student         If one should use the student-t distribution (default: False)
  -p PERCENTILE, --percentile PERCENTILE
                        Percentile used for VaR calculations, for example input 99.9 equals a 99.9 Percent VaR
                        (default: 99.9)
  -h, --help            show this help message (default: False)
```

Example:

```
2022 Feb 16, 11:18 (๐ฆ) /stocks/qa/ $ var
          FB Value at Risk
โโโโโโโโโณโโโโโโโโโโณโโโโโโโโโโโโโโโโโโ
โ       โ VaR:    โ Historical VaR: โ
โกโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโฉ
โ 90.0% โ -0.0305 โ -0.0233         โ
โโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโโโโโโโโโค
โ 95.0% โ -0.0389 โ -0.0364         โ
โโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโโโโโโโโโค
โ 99.0% โ -0.0546 โ -0.0578         โ
โโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโโโโโโโโโค
โ 99.9% โ -0.0719 โ -0.1719         โ
โโโโโโโโโดโโโโโโโโโโดโโโโโโโโโโโโโโโโโโ
```
