---
title: greeks
description: OpenBB Terminal Function
---

# greeks

The greeks for a given option.

### Usage

```python
greeks [-d DIVIDEND] [-r RISK_FREE] [-p] [-m MIN] [-M MAX] [-a]
```

---

## Parameters

| Name | Description | Default | Optional | Choices |
| ---- | ----------- | ------- | -------- | ------- |
| dividend | The dividend continuous rate | 0 | True | None |
| risk_free | The risk free rate | None | True | None |
| put | Whether the option is a put. | False | True | None |
| min | Minimum strike price to show. | None | True | None |
| max | Maximum strike price to show. | None | True | None |
| all | Whether to show all greeks. | False | True | None |


---

## Examples

```python
2022 Feb 16, 08:52 (๐ฆ) /stocks/options/ $ greeks -a
                                            Greeks
โโโโโโโโโโโณโโโโโโโโโโโโโโณโโโโโโโโณโโโโโโโโณโโโโโโโณโโโโโโโโณโโโโโโโณโโโโโโโโณโโโโโโโโณโโโโโโโโณโโโโโโโโ
โ Strike  โ Implied Vol โ Delta โ Gamma โ Vega โ Theta โ Rho  โ Phi   โ Charm โ Vanna โ Vomma โ
โกโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโฉ
โ 690.00  โ 0.00        โ 1.00  โ 0.00  โ 0.00 โ -0.00 โ 0.01 โ -0.01 โ 0.00  โ -0.00 โ -0.00 โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 700.00  โ 0.00        โ 1.00  โ 0.00  โ 0.00 โ -0.00 โ 0.01 โ -0.01 โ 0.00  โ -0.00 โ -0.00 โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 710.00  โ 0.00        โ 1.00  โ 0.00  โ 0.00 โ -0.00 โ 0.01 โ -0.01 โ 0.00  โ -0.00 โ -0.00 โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 720.00  โ 0.00        โ 1.00  โ 0.00  โ 0.00 โ -0.00 โ 0.01 โ -0.01 โ 0.00  โ -0.00 โ -0.00 โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 725.00  โ 0.00        โ 1.00  โ 0.00  โ 0.00 โ -0.00 โ 0.01 โ -0.01 โ 0.00  โ -0.00 โ -0.00 โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 730.00  โ 0.00        โ 1.00  โ 0.00  โ 0.00 โ -0.00 โ 0.01 โ -0.01 โ 0.00  โ -0.00 โ -0.00 โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 740.00  โ 0.00        โ 1.00  โ 0.00  โ 0.00 โ -0.00 โ 0.01 โ -0.01 โ 0.00  โ -0.00 โ -0.00 โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 750.00  โ 0.00        โ 1.00  โ 0.00  โ 0.00 โ -0.00 โ 0.01 โ -0.01 โ 0.00  โ -0.00 โ -0.00 โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 760.00  โ 0.00        โ 1.00  โ 0.00  โ 0.00 โ -0.00 โ 0.01 โ -0.01 โ 0.00  โ -0.00 โ -0.00 โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 770.00  โ 0.00        โ 1.00  โ 0.00  โ 0.00 โ -0.00 โ 0.01 โ -0.01 โ 0.00  โ -0.00 โ -0.00 โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 775.00  โ 0.00        โ 1.00  โ 0.00  โ 0.00 โ -0.00 โ 0.01 โ -0.01 โ 0.00  โ -0.00 โ -0.00 โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 780.00  โ 0.00        โ 1.00  โ 0.00  โ 0.00 โ -0.00 โ 0.01 โ -0.01 โ 0.00  โ -0.00 โ -0.00 โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 790.00  โ 0.00        โ 1.00  โ 0.00  โ 0.00 โ -0.00 โ 0.01 โ -0.01 โ 0.00  โ -0.00 โ -0.00 โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 800.00  โ 0.00        โ 1.00  โ 0.00  โ 0.00 โ -0.00 โ 0.01 โ -0.01 โ 0.00  โ -0.00 โ -0.00 โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 825.00  โ 0.00        โ 1.00  โ 0.00  โ 0.00 โ -0.00 โ 0.01 โ -0.01 โ 0.00  โ -0.00 โ -0.00 โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 850.00  โ 0.00        โ 1.00  โ 0.00  โ 0.00 โ -0.00 โ 0.01 โ -0.01 โ 0.00  โ -0.00 โ -0.00 โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 875.00  โ 0.00        โ 1.00  โ 0.00  โ 0.00 โ -0.00 โ 0.01 โ -0.01 โ 0.00  โ -0.00 โ -0.00 โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 900.00  โ 0.00        โ 1.00  โ 0.00  โ 0.00 โ -0.00 โ 0.01 โ -0.01 โ 0.00  โ -0.00 โ -0.00 โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 925.00  โ 0.00        โ 0.00  โ 0.00  โ 0.00 โ 0.00  โ 0.00 โ -0.00 โ -0.00 โ 0.00  โ 0.00  โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 950.00  โ 0.02        โ 0.00  โ 0.00  โ 0.00 โ 0.00  โ 0.00 โ -0.00 โ -0.00 โ 0.00  โ 0.00  โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 975.00  โ 0.03        โ 0.00  โ 0.00  โ 0.00 โ 0.00  โ 0.00 โ -0.00 โ -0.00 โ 0.00  โ 0.00  โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 1000.00 โ 0.03        โ 0.00  โ 0.00  โ 0.00 โ 0.00  โ 0.00 โ -0.00 โ -0.00 โ 0.00  โ 0.00  โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 1025.00 โ 0.06        โ 0.00  โ 0.00  โ 0.00 โ 0.00  โ 0.00 โ -0.00 โ -0.00 โ 0.00  โ 0.00  โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 1050.00 โ 0.06        โ 0.00  โ 0.00  โ 0.00 โ 0.00  โ 0.00 โ -0.00 โ -0.00 โ 0.00  โ 0.00  โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 1075.00 โ 0.06        โ 0.00  โ 0.00  โ 0.00 โ 0.00  โ 0.00 โ -0.00 โ -0.00 โ 0.00  โ 0.00  โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 1100.00 โ 0.06        โ 0.00  โ 0.00  โ 0.00 โ 0.00  โ 0.00 โ -0.00 โ -0.00 โ 0.00  โ 0.00  โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 1105.00 โ 0.06        โ 0.00  โ 0.00  โ 0.00 โ 0.00  โ 0.00 โ -0.00 โ -0.00 โ 0.00  โ 0.00  โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 1110.00 โ 0.06        โ 0.00  โ 0.00  โ 0.00 โ 0.00  โ 0.00 โ -0.00 โ -0.00 โ 0.00  โ 0.00  โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 1115.00 โ 0.13        โ 0.00  โ 0.00  โ 0.00 โ 0.00  โ 0.00 โ -0.00 โ -0.00 โ 0.00  โ 0.00  โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 1120.00 โ 0.13        โ 0.00  โ 0.00  โ 0.00 โ 0.00  โ 0.00 โ -0.00 โ -0.00 โ 0.00  โ 0.00  โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 1125.00 โ 0.13        โ 0.00  โ 0.00  โ 0.00 โ 0.00  โ 0.00 โ -0.00 โ -0.00 โ 0.00  โ 0.00  โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 1130.00 โ 0.13        โ 0.00  โ 0.00  โ 0.00 โ 0.00  โ 0.00 โ -0.00 โ -0.00 โ 0.00  โ 0.00  โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 1135.00 โ 0.13        โ 0.00  โ 0.00  โ 0.00 โ 0.00  โ 0.00 โ -0.00 โ -0.00 โ 0.00  โ 0.00  โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 1140.00 โ 0.13        โ 0.00  โ 0.00  โ 0.00 โ 0.00  โ 0.00 โ -0.00 โ -0.00 โ 0.00  โ 0.00  โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 1145.00 โ 0.13        โ 0.00  โ 0.00  โ 0.00 โ 0.00  โ 0.00 โ -0.00 โ -0.00 โ 0.00  โ 0.00  โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 1150.00 โ 0.13        โ 0.00  โ 0.00  โ 0.00 โ 0.00  โ 0.00 โ -0.00 โ -0.00 โ 0.00  โ 0.00  โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 1155.00 โ 0.13        โ 0.00  โ 0.00  โ 0.00 โ 0.00  โ 0.00 โ -0.00 โ -0.00 โ 0.00  โ 0.00  โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 1160.00 โ 0.13        โ 0.00  โ 0.00  โ 0.00 โ 0.00  โ 0.00 โ -0.00 โ -0.00 โ 0.00  โ 0.00  โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 1165.00 โ 0.13        โ 0.00  โ 0.00  โ 0.00 โ 0.00  โ 0.00 โ -0.00 โ -0.00 โ 0.00  โ 0.00  โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 1170.00 โ 0.13        โ 0.00  โ 0.00  โ 0.00 โ 0.00  โ 0.00 โ -0.00 โ -0.00 โ 0.00  โ 0.00  โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 1175.00 โ 0.13        โ 0.00  โ 0.00  โ 0.00 โ 0.00  โ 0.00 โ -0.00 โ -0.00 โ 0.00  โ 0.00  โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 1180.00 โ 0.13        โ 0.00  โ 0.00  โ 0.00 โ 0.00  โ 0.00 โ -0.00 โ -0.00 โ 0.00  โ 0.00  โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 1185.00 โ 0.13        โ 0.00  โ 0.00  โ 0.00 โ 0.00  โ 0.00 โ -0.00 โ -0.00 โ 0.00  โ 0.00  โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 1190.00 โ 0.13        โ 0.00  โ 0.00  โ 0.00 โ 0.00  โ 0.00 โ -0.00 โ -0.00 โ 0.00  โ 0.00  โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 1195.00 โ 0.13        โ 0.00  โ 0.00  โ 0.00 โ 0.00  โ 0.00 โ -0.00 โ -0.00 โ 0.00  โ 0.00  โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 1200.00 โ 0.13        โ 0.00  โ 0.00  โ 0.00 โ 0.00  โ 0.00 โ -0.00 โ -0.00 โ 0.00  โ 0.00  โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 1205.00 โ 0.13        โ 0.00  โ 0.00  โ 0.00 โ 0.00  โ 0.00 โ -0.00 โ -0.00 โ 0.00  โ 0.00  โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 1210.00 โ 0.13        โ 0.00  โ 0.00  โ 0.00 โ 0.00  โ 0.00 โ -0.00 โ -0.00 โ 0.00  โ 0.00  โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 1215.00 โ 0.13        โ 0.00  โ 0.00  โ 0.00 โ 0.00  โ 0.00 โ -0.00 โ -0.00 โ 0.00  โ 0.00  โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 1220.00 โ 0.13        โ 0.00  โ 0.00  โ 0.00 โ 0.00  โ 0.00 โ -0.00 โ -0.00 โ 0.00  โ 0.00  โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 1225.00 โ 0.13        โ 0.00  โ 0.00  โ 0.00 โ 0.00  โ 0.00 โ -0.00 โ -0.00 โ 0.00  โ 0.00  โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 1230.00 โ 0.13        โ 0.00  โ 0.00  โ 0.00 โ 0.00  โ 0.00 โ -0.00 โ -0.00 โ 0.00  โ 0.00  โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 1235.00 โ 0.13        โ 0.00  โ 0.00  โ 0.00 โ 0.00  โ 0.00 โ -0.00 โ -0.00 โ 0.00  โ 0.00  โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 1240.00 โ 0.13        โ 0.00  โ 0.00  โ 0.00 โ 0.00  โ 0.00 โ -0.00 โ -0.00 โ 0.00  โ 0.00  โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 1245.00 โ 0.13        โ 0.00  โ 0.00  โ 0.00 โ 0.00  โ 0.00 โ -0.00 โ -0.00 โ 0.00  โ 0.00  โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 1250.00 โ 0.13        โ 0.00  โ 0.00  โ 0.00 โ 0.00  โ 0.00 โ -0.00 โ -0.00 โ 0.00  โ 0.00  โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 1255.00 โ 0.13        โ 0.00  โ 0.00  โ 0.00 โ 0.00  โ 0.00 โ -0.00 โ -0.00 โ 0.00  โ 0.00  โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 1260.00 โ 0.13        โ 0.00  โ 0.00  โ 0.00 โ 0.00  โ 0.00 โ -0.00 โ -0.00 โ 0.00  โ 0.00  โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 1265.00 โ 0.13        โ 0.00  โ 0.00  โ 0.00 โ 0.00  โ 0.00 โ -0.00 โ -0.00 โ 0.00  โ 0.00  โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 1270.00 โ 0.13        โ 0.00  โ 0.00  โ 0.00 โ 0.00  โ 0.00 โ -0.00 โ -0.00 โ 0.00  โ 0.00  โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 1275.00 โ 0.13        โ 0.00  โ 0.00  โ 0.00 โ 0.00  โ 0.00 โ -0.00 โ -0.00 โ 0.00  โ 0.00  โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 1280.00 โ 0.13        โ 0.00  โ 0.00  โ 0.00 โ 0.00  โ 0.00 โ -0.00 โ -0.00 โ 0.00  โ 0.00  โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 1285.00 โ 0.13        โ 0.00  โ 0.00  โ 0.00 โ 0.00  โ 0.00 โ -0.00 โ -0.00 โ 0.00  โ 0.00  โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 1290.00 โ 0.13        โ 0.00  โ 0.00  โ 0.00 โ 0.00  โ 0.00 โ -0.00 โ -0.00 โ 0.00  โ 0.00  โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 1295.00 โ 0.13        โ 0.00  โ 0.00  โ 0.00 โ 0.00  โ 0.00 โ -0.00 โ -0.00 โ 0.00  โ 0.00  โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 1300.00 โ 0.13        โ 0.00  โ 0.00  โ 0.00 โ 0.00  โ 0.00 โ -0.00 โ -0.00 โ 0.00  โ 0.00  โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 1325.00 โ 0.13        โ 0.00  โ 0.00  โ 0.00 โ 0.00  โ 0.00 โ -0.00 โ -0.00 โ 0.00  โ 0.00  โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 1350.00 โ 0.13        โ 0.00  โ 0.00  โ 0.00 โ 0.00  โ 0.00 โ -0.00 โ -0.00 โ 0.00  โ 0.00  โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 1375.00 โ 0.25        โ 0.00  โ 0.00  โ 0.00 โ 0.00  โ 0.00 โ -0.00 โ -0.00 โ 0.00  โ 0.00  โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 1400.00 โ 0.25        โ 0.00  โ 0.00  โ 0.00 โ 0.00  โ 0.00 โ -0.00 โ -0.00 โ 0.00  โ 0.00  โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 1425.00 โ 0.25        โ 0.00  โ 0.00  โ 0.00 โ 0.00  โ 0.00 โ -0.00 โ -0.00 โ 0.00  โ 0.00  โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 1450.00 โ 0.25        โ 0.00  โ 0.00  โ 0.00 โ 0.00  โ 0.00 โ -0.00 โ -0.00 โ 0.00  โ 0.00  โ
โโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโผโโโโโโโโค
โ 1475.00 โ 0.25        โ 0.00  โ 0.00  โ 0.00 โ 0.00  โ 0.00 โ -0.00 โ -0.00 โ 0.00  โ 0.00  โ
โโโโโโโโโโโดโโโโโโโโโโโโโโดโโโโโโโโดโโโโโโโโดโโโโโโโดโโโโโโโโดโโโโโโโดโโโโโโโโดโโโโโโโโดโโโโโโโโดโโโโโโโโ
```
---
