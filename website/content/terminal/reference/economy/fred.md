---
title: fred
description: OpenBB Terminal Function
---

# fred

Query the FRED database and plot data based on the Series ID. [Source: FRED]

### Usage

```python
fred [-p PARAMETER] [-s START_DATE] [-e END_DATE] [-q QUERY]
```

---

## Parameters

| Name | Description | Default | Optional | Choices |
| ---- | ----------- | ------- | -------- | ------- |
| parameter | Series ID of the Macro Economic data from FRED |  | True | None |
| start_date | Starting date (YYYY-MM-DD) of data | None | True | None |
| end_date | Ending date (YYYY-MM-DD) of data | None | True | None |
| query | Query the FRED database to obtain Series IDs given the query search term. | None | True | None |


---

## Examples

```python
2022 Mar 15, 07:08 (๐ฆ) /economy/ $ fred -q treasuries
                                                                    Search results for treasuries
โโโโโโโโโโโโโณโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโณโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโ
โ Series ID โ Title                                           โ Description                                                                                         โ
โกโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโฉ
โ T10Y2Y    โ 10-Year Treasury Constant Maturity Minus 2-Year โ Starting with the update on June 21, 2019, the Treasury bond data used in calculating interest rate โ
โ           โ Treasury Constant Maturity                      โ spreads is obtained directly from the U.S. Treasury Department (https://www.treasury.gov/resource-  โ
โ           โ                                                 โ center/data-chart-center/interest-rates/Pages/TextView.aspx?data=yield).  Series is calculated as   โ
โ           โ                                                 โ the spread between 10-Year Treasury Constant Maturity (BC_10YEAR) and 2-Year Treasury Constant      โ
โ           โ                                                 โ Maturity (BC_2YEAR). Both underlying series are published at the U.S. Treasury Department           โ
โ           โ                                                 โ (https://www.treasury.gov/resource-center/data-chart-center/interest-                               โ
โ           โ                                                 โ rates/Pages/TextView.aspx?data=yield).                                                              โ
โโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโค
โ T10Y2YM   โ 10-Year Treasury Constant Maturity Minus 2-Year โ Series is calculated as the spread between 10-Year Treasury Constant Maturity (BC_10YEARM) and      โ
โ           โ Treasury Constant Maturity                      โ 2-Year Treasury Constant Maturity (BC_2YEARM). Starting with the update on June 21, 2019, the       โ
โ           โ                                                 โ Treasury bond data used in calculating interest rate spreads is obtained directly from the U.S.     โ
โ           โ                                                 โ Treasury Department (https://www.treasury.gov/resource-center/data-chart-center/interest-           โ
โ           โ                                                 โ rates/Pages/TextView.aspx?data=yield).                                                              โ
โโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโค
โ DFII10    โ Market Yield on U.S. Treasury Securities at     โ For further information regarding treasury constant maturity data, please refer to the Board of     โ
โ           โ 10-Year Constant Maturity, Inflation-Indexed    โ Governors ( http://www.federalreserve.gov/releases/h15/current/h15.pdf) and the Treasury            โ
โ           โ                                                 โ (http://www.treasury.gov/resource-center/data-chart-center/interest-rates/Pages/yieldmethod.aspx).  โ
โโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโค
โ FII10     โ Market Yield on U.S. Treasury Securities at     โ For further information regarding treasury constant maturity data, please refer to                  โ
โ           โ 10-Year Constant Maturity, Inflation-Indexed    โ http://www.federalreserve.gov/releases/h15/current/h15.pdf and http://www.treasury.gov/resource-    โ
โ           โ                                                 โ center/data-chart-center/interest-rates/Pages/yieldmethod.aspx.                                     โ
โโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโค
โ WFII10    โ Market Yield on U.S. Treasury Securities at     โ For further information regarding treasury constant maturity data, please refer to                  โ
โ           โ 10-Year Constant Maturity, Inflation-Indexed    โ http://www.federalreserve.gov/releases/h15/current/h15.pdf and http://www.treasury.gov/resource-    โ
โ           โ                                                 โ center/data-chart-center/interest-rates/Pages/yieldmethod.aspx.                                     โ
โโโโโโโโโโโโโดโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโดโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโ
```
![fred](https://user-images.githubusercontent.com/46355364/158575129-1d4b26de-8bd8-49b3-b1b9-e349afaf8a50.png)

---
