---
title: rmv
description: OpenBB Terminal Function
---

# rmv

Remove one of the options to be shown in the hedge.

### Usage

```python
rmv [-o OPTION [OPTION ...]] [-a]
```

---

## Parameters

| Name | Description | Default | Optional | Choices |
| ---- | ----------- | ------- | -------- | ------- |
| option | index of the option to remove | None | True | None |
| all | remove all of the options | False | True | None |


---

## Examples

```python
2022 May 10, 09:32 (๐ฆ) /stocks/options/hedge/ $ rmv Option A
          Current Option Positions           
โโโโโโโโณโโโโโโโณโโโโโโโโโณโโโโโโโโโโโโโโโโโโโโโ
โ Type โ Hold โ Strike โ Implied Volatility โ
โกโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโฉ
โ Call โ Long โ 155.00 โ 0.06               โ
โโโโโโโโดโโโโโโโดโโโโโโโโโดโโโโโโโโโโโโโโโโโโโโโ
```
---
