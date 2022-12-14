```
usage: var [-m] [-a] [-s] [-p PERCENTILE] [-h]
```

Provides value at risk (short: VaR) of the selected portfolio.

```
optional arguments:
  -m, --mean            If one should use the mean of the portfolio return (default: False)
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
2022 Feb 25, 03:09 (๐ฆ) /portfolio/ $ var
       Portfolio Value at Risk
โโโโโโโโโณโโโโโโโโโโณโโโโโโโโโโโโโโโโโโ
โ       โ VaR:    โ Historical VaR: โ
โกโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโฉ
โ 90.0% โ -0.0148 โ -0.0135         โ
โโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโโโโโโโโโค
โ 95.0% โ -0.0189 โ -0.0197         โ
โโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโโโโโโโโโค
โ 99.0% โ -0.0267 โ -0.0258         โ
โโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโโโโโโโโโค
โ 99.9% โ -0.0353 โ -0.0276         โ
โโโโโโโโโดโโโโโโโโโโดโโโโโโโโโโโโโโโโโโ
```
