---
title: add
description: OpenBB Terminal Function
---

# add

Adds a price to the list

### Usage

```python
add -p PRICE -c CHANCE
```

---

## Parameters

| Name | Description | Default | Optional | Choices |
| ---- | ----------- | ------- | -------- | ------- |
| price | Projected price of the stock at the expiration date | None | False | None |
| chance | Chance that the stock is at a given projected price | None | False | None |


---

## Examples

```python
2022 Feb 16, 09:42 (๐ฆ) /stocks/options/pricing/ $ add -p 175 -c 0.5

2022 Feb 16, 09:43 (๐ฆ) /stocks/options/pricing/ $ add -p 165 -c 0.5

2022 Feb 16, 09:43 (๐ฆ) /stocks/options/pricing/ $ show
Estimated price(s) of AAPL at 2022-05-20
โโโโโโโโโโณโโโโโโโโโ
โ Price  โ Chance โ
โกโโโโโโโโโโโโโโโโโโฉ
โ 165.00 โ 0.50   โ
โโโโโโโโโโผโโโโโโโโโค
โ 175.00 โ 0.50   โ
โโโโโโโโโโดโโโโโโโโโ
```
---
