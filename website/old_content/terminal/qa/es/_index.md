```
usage: es [-m] [-d {laplace,student_t,logistic,normal}] [-p PERCENTILE] [-h]
```

Provides Expected Shortfall (short: ES) of the selected stock.

```
optional arguments:
  -m, --mean            If one should use the mean of the stocks return (default: False)
  -d {laplace,student_t,logistic,normal}, --dist {laplace,student_t,logistic,normal}, --distributions {laplace,student_t,logistic,normal}
                        Distribution used for the calculations (default: normal)
  -p PERCENTILE, --percentile PERCENTILE
                        Percentile used for ES calculations, for example input 99.9 equals a 99.9 Percent Expected
                        Shortfall (default: 99.9)
  -h, --help            show this help message (default: False)
```

Example:

```
2022 Feb 25, 06:50 (๐ฆ) /stocks/qa/ $ es
      TSLA Expected Shortfall
โโโโโโโโโณโโโโโโโโโโณโโโโโโโโโโโโโโโโโ
โ       โ ES:     โ Historical ES: โ
โกโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโฉ
โ 90.0% โ -0.0752 โ -0.0705        โ
โโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโโโโโโโโค
โ 95.0% โ -0.0885 โ -0.0932        โ
โโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโโโโโโโโค
โ 99.0% โ -0.1144 โ -0.1561        โ
โโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโโโโโโโโค
โ 99.9% โ -0.1444 โ -0.2106        โ
โโโโโโโโโดโโโโโโโโโโดโโโโโโโโโโโโโโโโโ
```
