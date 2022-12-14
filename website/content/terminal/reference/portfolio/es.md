---
title: es
description: OpenBB Terminal Function
---

# es

Provides Expected Shortfall (short: ES) of the selected portfolio.

### Usage

```python
es [-m] [-d DIST] [-p PERCENTILE]
```

---

## Parameters

| Name | Description | Default | Optional | Choices |
| ---- | ----------- | ------- | -------- | ------- |
| use_mean | If one should use the mean of the portfolios return | True | True | None |
| distribution | Distribution used for the calculations | normal | True | laplace, student_t, logistic, normal |
| percentile | Percentile used for ES calculations, for example input 99.9 equals a 99.9 Percent Expected Shortfall | 99.9 | True | None |


---

## Examples

```python
2022 Feb 25, 03:09 (๐ฆ) /portfolio/ $ es
    Portfolio Expected Shortfall
โโโโโโโโโณโโโโโโโโโโณโโโโโโโโโโโโโโโโโ
โ       โ ES:     โ Historical ES: โ
โกโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโฉ
โ 90.0% โ -0.0204 โ -0.0202        โ
โโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโโโโโโโโค
โ 95.0% โ -0.0240 โ -0.0242        โ
โโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโโโโโโโโค
โ 99.0% โ -0.0310 โ -0.0270        โ
โโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโโโโโโโโค
โ 99.9% โ -0.0391 โ -0.0277        โ
โโโโโโโโโดโโโโโโโโโโดโโโโโโโโโโโโโโโโโ
```
---
