---
title: alloc
description: OpenBB Terminal Function
---

# alloc

Show your allocation to each asset or sector compared to the benchmark.

### Usage

```python
alloc [-a AGG] [-t]
```

---

## Parameters

| Name | Description | Default | Optional | Choices |
| ---- | ----------- | ------- | -------- | ------- |
| agg | The type of allocation aggregation you wish to do | assets | True | assets, sectors, countries, regions |
| tables | Whether to also include the assets/sectors tables of both the benchmark and the portfolio. | False | True | None |


---

## Examples

```python
022 May 12, 06:23 (๐ฆ) /portfolio/ $ alloc assets
Portfolio vs. Benchmark - Top 10 Assets Allocation
โโโโโโโโโโณโโโโโโโโโโโโณโโโโโโโโโโโโณโโโโโโโโโโโโโ
โ Symbol โ Portfolio โ Benchmark โ Difference โ
โกโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโฉ
โ ASML   โ 24.44%    โ 0.00e+00  โ 24.44%     โ
โโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโโโค
โ AMZN   โ 21.96%    โ 3.33%     โ 18.63%     โ
โโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโโโค
โ GOOGL  โ 18.94%    โ 1.66%     โ 17.28%     โ
โโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโโโค
โ TSM    โ 9.43%     โ 0.00e+00  โ 9.43%      โ
โโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโโโค
โ DGX    โ 6.23%     โ 0.00e+00  โ 6.23%      โ
โโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโโโค
โ BABA   โ 5.54%     โ 0.00e+00  โ 5.54%      โ
โโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโโโค
โ APTV   โ 3.78%     โ 0.00e+00  โ 3.78%      โ
โโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโโโค
โ AAPL   โ 3.36%     โ 4.90%     โ -1.54%     โ
โโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโโโค
โ NKE    โ 3.26%     โ 0.00e+00  โ 3.26%      โ
โโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโโโค
โ YUM    โ 3.06%     โ 0.00e+00  โ 3.06%      โ
โโโโโโโโโโดโโโโโโโโโโโโดโโโโโโโโโโโโดโโโโโโโโโโโโโ

2022 May 12, 06:23 (๐ฆ) /portfolio/ $ alloc sectors

      Portfolio vs. Benchmark - Top 4 Sectors Allocation       
โโโโโโโโโโโโโโโโโโโโโโโโโโณโโโโโโโโโโโโณโโโโโโโโโโโโณโโโโโโโโโโโโโ
โ Sectors                โ Portfolio โ Benchmark โ Difference โ
โกโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโฉ
โ Technology             โ 59.19%    โ 24.95%    โ 34.24%     โ
โโโโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโโโค
โ Communication Services โ 18.94%    โ 8.55%     โ 10.39%     โ
โโโโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโโโค
โ Consumer Cyclical      โ 15.64%    โ 11.55%    โ 4.09%      โ
โโโโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโโโค
โ Healthcare             โ 6.23%     โ 13.41%    โ -7.18%     โ
โโโโโโโโโโโโโโโโโโโโโโโโโโดโโโโโโโโโโโโดโโโโโโโโโโโโดโโโโโโโโโโโโโ

2022 May 12, 06:23 (๐ฆ) /portfolio/ $ alloc countries

 Portfolio vs. Benchmark - Top 5 Countries Allocation 
โโโโโโโโโโโโโโโโโณโโโโโโโโโโโโณโโโโโโโโโโโโณโโโโโโโโโโโโโ
โ Countries     โ Portfolio โ Benchmark โ Difference โ
โกโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโฉ
โ United States โ 57.33%    โ 99.17%    โ -41.84%    โ
โโโโโโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโโโค
โ Netherlands   โ 24.44%    โ 0.00e+00  โ 24.44%     โ
โโโโโโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโโโค
โ Taiwan        โ 9.43%     โ 1.00e-04  โ 9.42%      โ
โโโโโโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโโโค
โ China         โ 5.54%     โ 0.00e+00  โ 5.54%      โ
โโโโโโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโโโค
โ Germany       โ 3.26%     โ 0.00e+00  โ 3.26%      โ
โโโโโโโโโโโโโโโโโดโโโโโโโโโโโโดโโโโโโโโโโโโดโโโโโโโโโโโโโ

2022 May 12, 06:23 (๐ฆ) /portfolio/ $ alloc regions

  Portfolio vs. Benchmark - Top 3 Regions Allocation  
โโโโโโโโโโโโโโโโโณโโโโโโโโโโโโณโโโโโโโโโโโโณโโโโโโโโโโโโโ
โ Regions       โ Portfolio โ Benchmark โ Difference โ
โกโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโฉ
โ North America โ 57.33%    โ 99.25%    โ -41.92%    โ
โโโโโโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโโโค
โ Europe        โ 27.70%    โ 0.64%     โ 27.06%     โ
โโโโโโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโโโค
โ Asia          โ 14.96%    โ 7.00e-04  โ 14.89%     โ
โโโโโโโโโโโโโโโโโดโโโโโโโโโโโโดโโโโโโโโโโโโดโโโโโโโโโโโโโ
```
---
