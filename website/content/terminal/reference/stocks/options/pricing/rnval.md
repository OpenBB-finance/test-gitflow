---
title: rnval
description: OpenBB Terminal Function
---

# rnval

The risk neutral value of the options

### Usage

```python
rnval [-p] [-m MINI] [-M MAXI] [-r RISK]
```

---

## Parameters

| Name | Description | Default | Optional | Choices |
| ---- | ----------- | ------- | -------- | ------- |
| put | Show puts instead of calls | False | True | None |
| mini | Minimum strike price shown | None | True | None |
| maxi | Maximum strike price shown | None | True | None |
| risk | The risk-free rate to use | None | True | None |


---

## Examples

```python
2022 Feb 16, 09:45 (๐ฆ) /stocks/options/pricing/ $ add -p 100 -c 0.5

2022 Feb 16, 09:46 (๐ฆ) /stocks/options/pricing/ $ add -p 200 -c 0.5

2022 Feb 16, 09:46 (๐ฆ) /stocks/options/pricing/ $ show
Estimated price(s) of AAPL at 2022-05-20
โโโโโโโโโโณโโโโโโโโโ
โ Price  โ Chance โ
โกโโโโโโโโโโโโโโโโโโฉ
โ 100.00 โ 0.50   โ
โโโโโโโโโโผโโโโโโโโโค
โ 200.00 โ 0.50   โ
โโโโโโโโโโดโโโโโโโโโ
2022 Feb 16, 09:46 (๐ฆ) /stocks/options/pricing/ $ rnval
            Risk Neutral Values
โโโโโโโโโโณโโโโโโโโโโโโโณโโโโโโโโณโโโโโโโโโโโโโ
โ Strike โ Last Price โ Value โ Difference โ
โกโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโฉ
โ 120.00 โ 53.25      โ 39.99 โ 13.26      โ
โโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโโโโโโค
โ 125.00 โ 48.11      โ 37.49 โ 10.62      โ
โโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโโโโโโค
โ 130.00 โ 43.80      โ 34.99 โ 8.81       โ
โโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโโโโโโค
โ 135.00 โ 37.71      โ 32.49 โ 5.22       โ
โโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโโโโโโค
โ 140.00 โ 35.00      โ 29.99 โ 5.01       โ
โโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโโโโโโค
โ 145.00 โ 30.35      โ 27.49 โ 2.86       โ
โโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโโโโโโค
โ 150.00 โ 26.30      โ 24.99 โ 1.31       โ
โโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโโโโโโค
โ 155.00 โ 22.35      โ 22.49 โ -0.14      โ
โโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโโโโโโค
โ 160.00 โ 18.30      โ 19.99 โ -1.69      โ
โโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโโโโโโค
โ 165.00 โ 15.00      โ 17.50 โ -2.50      โ
โโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโโโโโโค
โ 170.00 โ 11.35      โ 15.00 โ -3.65      โ
โโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโโโโโโค
โ 175.00 โ 8.65       โ 12.50 โ -3.85      โ
โโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโโโโโโค
โ 180.00 โ 6.70       โ 10.00 โ -3.30      โ
โโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโโโโโโค
โ 185.00 โ 4.60       โ 7.50  โ -2.90      โ
โโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโโโโโโค
โ 190.00 โ 3.25       โ 5.00  โ -1.75      โ
โโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโโโโโโค
โ 195.00 โ 2.29       โ 2.50  โ -0.21      โ
โโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโโโโโโค
โ 200.00 โ 1.59       โ 0.00  โ 1.59       โ
โโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโผโโโโโโโโโโโโโค
โ 210.00 โ 0.70       โ 0.00  โ 0.70       โ
โโโโโโโโโโดโโโโโโโโโโโโโดโโโโโโโโดโโโโโโโโโโโโโ
```
---
