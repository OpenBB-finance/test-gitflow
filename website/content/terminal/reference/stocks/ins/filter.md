---
title: filter
description: OpenBB Terminal Function
---

# filter

Print open insider filtered data using loaded preset. [Source: OpenInsider]

### Usage

```python
filter [-l LIMIT] [-u]
```

---

## Parameters

| Name | Description | Default | Optional | Choices |
| ---- | ----------- | ------- | -------- | ------- |
| limit | Limit of datarows to display | 10 | True | None |
| urls | Flag to show hyperlinks | False | True | None |


---

## Examples

```python
2022 Feb 16, 07:51 (๐ฆ) /stocks/ins/ $ filter
                                                                                  Insider filtered
โโโโโณโโโโโโโโโโโโโโโณโโโโโโโโโณโโโโโโโโโโโโโโโโโโโโโโโโณโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโณโโโโโโโโโโณโโโโโโโโโโโโโโณโโโโโโโโโโโโโโณโโโโโโโโโโโโณโโโโโโโโโโโโโโโโโโณโโโโโโโโโโโโโโโโโโโโโโโโโโโโโ
โ X โ Trading Date โ Ticker โ Insider               โ Title                        โ Price   โ Quantity    โ Owned       โ Delta Own โ Value           โ Company                    โ
โกโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโฉ
โ   โ 2022-02-14   โ MGM    โ Meister Keith A.      โ Dir                          โ $45.00  โ -4,500,000  โ 6,673,778   โ -40%      โ -$202,500,000   โ Mgm Resorts International  โ
โโโโโผโโโโโโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโโโโโโโค
โ M โ 2022-02-10   โ MA     โ Mastercard Foundation โ 10%                          โ $375.58 โ -465,180    โ 104,471,071 โ 0%        โ -$174,712,785   โ Mastercard Inc             โ
โโโโโผโโโโโโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโโโโโโโค
โ D โ 2022-02-10   โ EL     โ Lauder Ronald S       โ COB, Clinique Labs, LLC, 10% โ $307.08 โ -700,000    โ 6,364       โ -99%      โ -$214,956,000   โ Estee Lauder Companies Inc โ
โโโโโผโโโโโโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโโโโโโโค
โ M โ 2022-02-07   โ MA     โ Mastercard Foundation โ 10%                          โ $378.65 โ -465,180    โ 104,936,251 โ 0%        โ -$176,139,632   โ Mastercard Inc             โ
โโโโโผโโโโโโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโโโโโโโค
โ   โ 2022-02-04   โ VIRT   โ Gic Private Ltd       โ 10%                          โ $31.04  โ -4,027,062  โ 8,731,144   โ -32%      โ -$125,000,004   โ Virtu Financial, Inc.      โ
โโโโโผโโโโโโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโโโโโโโค
โ D โ 2022-02-04   โ BKR    โ General Electric Co   โ 10%                          โ $25.98  โ -50,097,840 โ 116,548,079 โ -30%      โ -$1,301,541,883 โ Baker Hughes Co            โ
โโโโโผโโโโโโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโโโโโโโค
โ D โ 2022-02-03   โ MGY    โ Enervest, Ltd.        โ Dir, 10%                     โ $21.00  โ -7,455,815  โ 16,282,900  โ -31%      โ -$156,572,115   โ Magnolia Oil & Gas Corp    โ
โโโโโผโโโโโโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโโโโโโโค
โ D โ 2022-02-03   โ MGY    โ Walker John B         โ Dir, 10%                     โ $21.00  โ -7,455,815  โ 16,879,220  โ -31%      โ -$156,572,115   โ Magnolia Oil & Gas Corp    โ
โโโโโดโโโโโโโโโโโโโโโดโโโโโโโโโดโโโโโโโโโโโโโโโโโโโโโโโโดโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโดโโโโโโโโโโดโโโโโโโโโโโโโโดโโโโโโโโโโโโโโดโโโโโโโโโโโโดโโโโโโโโโโโโโโโโโโดโโโโโโโโโโโโโโโโโโโโโโโโโโโโโ

D: Derivative transaction in filing (usually option exercise)
M: Multiple transactions in filing; earliest reported transaction date & weighted average transaction price

S - Sale: Sale of securities on an exchange or to another person
S - Sale+OE: Sale of securities on an exchange or to another person (after option exercise)
```
---
