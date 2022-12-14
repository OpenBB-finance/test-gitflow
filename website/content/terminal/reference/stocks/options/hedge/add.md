---
title: add
description: OpenBB Terminal Function
---

# add

Add options to the diagram.

### Usage

```python
add [-p] [-s] -i {0,1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,46,47,48,49,50,51,52,53,54,55,56,57,58,59}
```

---

## Parameters

| Name | Description | Default | Optional | Choices |
| ---- | ----------- | ------- | -------- | ------- |
| put | Buy a put instead of a call | False | True | None |
| short | Short the option instead of buying it | False | True | None |
| identifier | The identifier of the option as found in the list command | None | False | range(0, 60) |


---

## Examples

```python
2022 May 10, 09:17 (๐ฆ) /stocks/options/hedge/ $ add 25
โโโโโโโโโโโโโโโโโโโโโโณโโโโโโโโโโโโ
โ                    โ Positions โ
โกโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโฉ
โ Delta              โ 1.00      โ
โโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโค
โ Gamma              โ 7253.89   โ
โโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโค
โ Vega               โ 0.14      โ
โโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโค
โ Implied Volatility โ 1.00e-05  โ
โโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโค
โ Strike Price       โ 147.00    โ
โโโโโโโโโโโโโโโโโโโโโโดโโโโโโโโโโโโ

          Current Option Positions           
โโโโโโโโณโโโโโโโณโโโโโโโโโณโโโโโโโโโโโโโโโโโโโโโ
โ Type โ Hold โ Strike โ Implied Volatility โ
โกโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโฉ
โ Call โ Long โ 147.00 โ 1.00e-05           โ
โโโโโโโโดโโโโโโโดโโโโโโโโโดโโโโโโโโโโโโโโโโโโโโโ
```
---
