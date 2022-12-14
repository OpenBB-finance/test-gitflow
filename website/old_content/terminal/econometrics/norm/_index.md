```
usage: norm [-c {OPTIONS}] [-h] [--export {csv,json,xlsx,png,jpg,pdf,svg}]
```

Test whether the used data is normally distributed.

Normal distribution, also known as the Gaussian distribution, is a probability distribution that is symmetric about the mean, showing that data near the mean are more frequent in occurrence than data far from the mean. In graph form, normal distribution will appear as a bell curve. [Source: Investopedia]

```
optional arguments:
  -c {OPTIONS}, --column {OPTIONS}
                        The column and name of the database you want to test normality for (default: None)
  -p, --plot            Whether you wish to plot a histogram to visually depict normality (default: False)
  -h, --help            show this help message (default: False)
  --export {csv,json,xlsx,png,jpg,pdf,svg}
                        Export raw data into csv, json, xlsx and figure into png, jpg, pdf, svg (default: )
```

Example for stock data (which is not normally distributed):

```
2022 Feb 24, 05:31 (๐ฆ) /econometrics/ $ norm tsla.adj_close -p
                 Normality Test [Column: adj_close | Dataset: tsla]
โโโโโโโโโโโโโณโโโโโโโโโโโณโโโโโโโโโโโณโโโโโโโโโโโโโโณโโโโโโโโโโโโโโโณโโโโโโโโโโโโโโโโโโโโโ
โ           โ Kurtosis โ Skewness โ Jarque-Bera โ Shapiro-Wilk โ Kolmogorov-Smirnov โ
โกโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโฉ
โ Statistic โ -18.71   โ 4.85     โ 66.36       โ 0.88         โ 1.00               โ
โโโโโโโโโโโโโผโโโโโโโโโโโผโโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโค
โ p-value   โ 0.00     โ 0.00     โ 0.00        โ 0.00         โ 0.00               โ
โโโโโโโโโโโโโดโโโโโโโโโโโดโโโโโโโโโโโดโโโโโโโโโโโโโโดโโโโโโโโโโโโโโโดโโโโโโโโโโโโโโโโโโโโโ
```

![histogram_adj_close_tsla](https://user-images.githubusercontent.com/46355364/155514663-90cb210a-002a-49fe-b7d3-29d9f2aeb5ac.png)

Example for returns (which is usually normally distributed):

```
2022 Feb 24, 05:36 (๐ฆ) /econometrics/ $ norm msft.return -p
                   Normality Test [Column: return | Dataset: msft]
โโโโโโโโโโโโโณโโโโโโโโโโโณโโโโโโโโโโโณโโโโโโโโโโโโโโณโโโโโโโโโโโโโโโณโโโโโโโโโโโโโโโโโโโโโ
โ           โ Kurtosis โ Skewness โ Jarque-Bera โ Shapiro-Wilk โ Kolmogorov-Smirnov โ
โกโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโฉ
โ Statistic โ 7.89     โ -3.56    โ 336.34      โ 0.96         โ 0.48               โ
โโโโโโโโโโโโโผโโโโโโโโโโโผโโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโค
โ p-value   โ 0.00     โ 0.00     โ 0.00        โ 0.00         โ 0.00               โ
โโโโโโโโโโโโโดโโโโโโโโโโโดโโโโโโโโโโโดโโโโโโโโโโโโโโดโโโโโโโโโโโโโโโดโโโโโโโโโโโโโโโโโโโโโ
```

![histogram_returns_msft](https://user-images.githubusercontent.com/46355364/155514702-f46da473-b340-4d68-b31e-f96606c4ed00.png)
