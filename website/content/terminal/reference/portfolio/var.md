---
title: var
description: OpenBB Terminal Function
---

# var

Provides value at risk (short: VaR) of the selected portfolio.

### Usage

```python
var [-m] [-a] [-s] [-p PERCENTILE]
```

---

## Parameters

| Name | Description | Default | Optional | Choices |
| ---- | ----------- | ------- | -------- | ------- |
| use_mean | If one should use the mean of the portfolio return | True | True | None |
| adjusted | If the VaR should be adjusted for skew and kurtosis (Cornish-Fisher-Expansion) | False | True | None |
| student_t | If one should use the student-t distribution | False | True | None |
| percentile | Percentile used for VaR calculations, for example input 99.9 equals a 99.9 Percent VaR | 99.9 | True | None |


---

## Examples

```python
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
---
