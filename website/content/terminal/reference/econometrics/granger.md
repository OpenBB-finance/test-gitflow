---
title: granger
description: OpenBB Terminal Function
---

# granger

Show Granger causality between two timeseries

### Usage

```python
granger [-t Available time series] [-l LAGS] [-c CONFIDENCE]
```

---

## Parameters

| Name | Description | Default | Optional | Choices |
| ---- | ----------- | ------- | -------- | ------- |
| ts | Requires two time series, the first time series is assumed to be Granger-caused by the second time series. | None | True | None |
| lags | How many lags should be included | 3 | True | None |
| confidence | Set the confidence level | 0.05 | True | None |


---

## Examples

```python
2022 Jun 01, 06:35 (๐ฆ) /econometrics/ $ load strikes

2022 Jun 01, 06:36 (๐ฆ) /econometrics/ $ granger strikes.duration,strikes.iprod

Granger Causality Test [Y: strikes.duration | X: strikes.iprod | Lags: 3]
โโโโโโโโโโโโโโโโณโโโโโโโโโณโโโโโโโโโโณโโโโโโโโณโโโโโโโ
โ              โ F-test โ P-value โ Count โ Lags โ
โกโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโฉ
โ ssr_ftest    โ 0.81   โ 0.49    โ 52.00 โ 3.00 โ
โโโโโโโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโผโโโโโโโโผโโโโโโโค
โ ssr_chi2test โ 2.75   โ 0.43    โ -     โ 3    โ
โโโโโโโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโผโโโโโโโโผโโโโโโโค
โ lrtest       โ 2.69   โ 0.44    โ -     โ 3    โ
โโโโโโโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโผโโโโโโโโผโโโโโโโค
โ params_ftest โ 0.81   โ 0.49    โ 52.00 โ 3.00 โ
โโโโโโโโโโโโโโโโดโโโโโโโโโดโโโโโโโโโโดโโโโโโโโดโโโโโโโ

As the p-value of the F-test is 0.495, we can not reject the null hypothesis at the 0.05 confidence level.
```
---
