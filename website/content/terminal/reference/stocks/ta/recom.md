---
title: recom
description: OpenBB Terminal Function
---

# recom

Print tradingview recommendation based on technical indicators. [Source: Tradingview]

### Usage

```python
recom [-s {australia,brazil,cfd,crypto,euronext,forex,france,germany,hongkong,india,indonesia,malaysia,philippines,russia,ksa,rsa,korea,spain,sweden,taiwan,thailand,turkey,uk,america,vietnam}] [-e EXCHANGE] [-i {1m,5m,15m,1h,4h,1d,1W,1M}]
```

---

## Parameters

| Name | Description | Default | Optional | Choices |
| ---- | ----------- | ------- | -------- | ------- |
| screener | Screener. See https://python-tradingview-ta.readthedocs.io/en/latest/usage.html | america | True | australia, brazil, cfd, crypto, euronext, forex, france, germany, hongkong, india, indonesia, malaysia, philippines, russia, ksa, rsa, korea, spain, sweden, taiwan, thailand, turkey, uk, america, vietnam |
| exchange | Set exchange. For Forex use: 'FX_IDC', and for crypto use 'TVC'. See https://python-tradingview-ta.readthedocs.io/en/latest/usage.html. By default Alpha Vantage tries to get this data from the ticker. |  | True | None |
| interval | Interval, that corresponds to the recommendation given by tradingview based on technical indicators. See https://python-tradingview-ta.readthedocs.io/en/latest/usage.html |  | True | 1m, 5m, 15m, 1h, 4h, 1d, 1W, 1M |


---

## Examples

```python
2022 Feb 16, 11:31 (๐ฆ) /stocks/ta/ $ recom
               Ticker Recommendation
โโโโโโโโโโโณโโโโโโโโโโโโโโโโโณโโโโโโณโโโโโโโณโโโโโโโโโโ
โ         โ RECOMMENDATION โ BUY โ SELL โ NEUTRAL โ
โกโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโฉ
โ 1 month โ BUY            โ 15  โ 2    โ 9       โ
โโโโโโโโโโโผโโโโโโโโโโโโโโโโโผโโโโโโผโโโโโโโผโโโโโโโโโโค
โ 1 week  โ BUY            โ 14  โ 2    โ 10      โ
โโโโโโโโโโโผโโโโโโโโโโโโโโโโโผโโโโโโผโโโโโโโผโโโโโโโโโโค
โ 1 day   โ SELL           โ 5   โ 13   โ 8       โ
โโโโโโโโโโโผโโโโโโโโโโโโโโโโโผโโโโโโผโโโโโโโผโโโโโโโโโโค
โ 4 hours โ SELL           โ 4   โ 14   โ 8       โ
โโโโโโโโโโโผโโโโโโโโโโโโโโโโโผโโโโโโผโโโโโโโผโโโโโโโโโโค
โ 1 hour  โ SELL           โ 4   โ 13   โ 9       โ
โโโโโโโโโโโผโโโโโโโโโโโโโโโโโผโโโโโโผโโโโโโโผโโโโโโโโโโค
โ 15 min  โ SELL           โ 3   โ 13   โ 10      โ
โโโโโโโโโโโผโโโโโโโโโโโโโโโโโผโโโโโโผโโโโโโโผโโโโโโโโโโค
โ 5 min   โ SELL           โ 5   โ 12   โ 9       โ
โโโโโโโโโโโผโโโโโโโโโโโโโโโโโผโโโโโโผโโโโโโโผโโโโโโโโโโค
โ 1 min   โ SELL           โ 6   โ 11   โ 9       โ
โโโโโโโโโโโดโโโโโโโโโโโโโโโโโดโโโโโโดโโโโโโโดโโโโโโโโโโ
```
---
