---
title: root
description: OpenBB Terminal Function
---

# root

Show unit root tests of a column of a dataset

### Usage

```python
root -v {} [-r {c,ct,ctt,n}] [-k {c,ct}]
```

---

## Parameters

| Name | Description | Default | Optional | Choices |
| ---- | ----------- | ------- | -------- | ------- |
| column | The column and name of the database you want test unit root for | None | False | None |
| fuller_reg | Type of regression. Can be 'c','ct','ctt','nc'. c - Constant and t - trend order | c | True | c, ct, ctt, n |
| kpss_reg | Type of regression. Can be 'c', 'ct'. c - Constant and t - trend order | c | True | c, ct |


---

## Examples

```python
2022 Jun 01, 06:47 (๐ฆ) /econometrics/ $ load fair

2022 Jun 01, 06:47 (๐ฆ) /econometrics/ $ root fair.yrs_married

Unitroot from dataset 'fair of 'yrs_married'
โโโโโโโโโโโโโโโโโโณโโโโโโโโโโโณโโโโโโโโ
โ                โ ADF      โ KPSS  โ
โกโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโฉ
โ Test Statistic โ -8.08    โ 7.01  โ
โโโโโโโโโโโโโโโโโโผโโโโโโโโโโโผโโโโโโโโค
โ P-Value        โ 0.00     โ 0.01  โ
โโโโโโโโโโโโโโโโโโผโโโโโโโโโโโผโโโโโโโโค
โ NLags          โ 34.00    โ 26.00 โ
โโโโโโโโโโโโโโโโโโผโโโโโโโโโโโผโโโโโโโโค
โ Nobs           โ 6331.00  โ 0.00  โ
โโโโโโโโโโโโโโโโโโผโโโโโโโโโโโผโโโโโโโโค
โ ICBest         โ 42958.72 โ 0.00  โ
โโโโโโโโโโโโโโโโโโดโโโโโโโโโโโดโโโโโโโโ
```
---
