---
title: var
description: OpenBB Terminal Function
---

# var

Provides value at risk (short: VaR) of the selected stock.

### Usage

```python
var [-m] [-a] [-s] [-p PERCENTILE] [-d DATA_RANGE]
```

---

## Parameters

| Name | Description | Default | Optional | Choices |
| ---- | ----------- | ------- | -------- | ------- |
| use_mean | If one should use the mean of the stocks return | False | True | None |
| adjusted | If the VaR should be adjusted for skew and kurtosis (Cornish-Fisher-Expansion) | False | True | None |
| student_t | If one should use the student-t distribution | False | True | None |
| percentile | Percentile used for VaR calculations, for example input 99.9 equals a 99.9 Percent VaR | 99.9 | True | None |
| data_range | Number of rows you want to use VaR over, ex: if you are using days, 30 would show VaR for the last 30 TRADING days | 0 | True | None |


---

## Examples

```python
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
---
