---
title: raw
description: OpenBB Terminal Function
---

# raw

Print raw data to console

### Usage

```python
raw [-l LIMIT] [-r] [-s {open,high,low,close,adjclose,volume,date_id,oc_high,oc_low,returns,logret,logprice}]
```

---

## Parameters

| Name | Description | Default | Optional | Choices |
| ---- | ----------- | ------- | -------- | ------- |
| limit | Number to show | 20 | True | None |
| reverse | Data is sorted in descending order by default. Reverse flag will sort it in an ascending way. Only works when raw data is displayed. | False | True | None |
| sortby | The column to sort by | None | True | open, high, low, close, adjclose, volume, date_id, oc_high, oc_low, returns, logret, logprice |


---

## Examples

```python
2022 Feb 16, 11:05 (๐ฆ) /stocks/qa/ $ raw
        Raw Data
โโโโโโโโโโโโโโณโโโโโโโโโโโ
โ            โ Adjclose โ
โกโโโโโโโโโโโโโโโโโโโโโโโโฉ
โ 2022-01-19 โ 995.650  โ
โโโโโโโโโโโโโโผโโโโโโโโโโโค
โ 2022-01-20 โ 996.270  โ
โโโโโโโโโโโโโโผโโโโโโโโโโโค
โ 2022-01-21 โ 943.900  โ
โโโโโโโโโโโโโโผโโโโโโโโโโโค
โ 2022-01-24 โ 930.000  โ
โโโโโโโโโโโโโโผโโโโโโโโโโโค
โ 2022-01-25 โ 918.400  โ
โโโโโโโโโโโโโโผโโโโโโโโโโโค
โ 2022-01-26 โ 937.410  โ
โโโโโโโโโโโโโโผโโโโโโโโโโโค
โ 2022-01-27 โ 829.100  โ
โโโโโโโโโโโโโโผโโโโโโโโโโโค
โ 2022-01-28 โ 846.350  โ
โโโโโโโโโโโโโโผโโโโโโโโโโโค
โ 2022-01-31 โ 936.720  โ
โโโโโโโโโโโโโโผโโโโโโโโโโโค
โ 2022-02-01 โ 931.250  โ
โโโโโโโโโโโโโโผโโโโโโโโโโโค
โ 2022-02-02 โ 905.660  โ
โโโโโโโโโโโโโโผโโโโโโโโโโโค
โ 2022-02-03 โ 891.140  โ
โโโโโโโโโโโโโโผโโโโโโโโโโโค
โ 2022-02-04 โ 923.320  โ
โโโโโโโโโโโโโโผโโโโโโโโโโโค
โ 2022-02-07 โ 907.340  โ
โโโโโโโโโโโโโโผโโโโโโโโโโโค
โ 2022-02-08 โ 922.000  โ
โโโโโโโโโโโโโโผโโโโโโโโโโโค
โ 2022-02-09 โ 932.000  โ
โโโโโโโโโโโโโโผโโโโโโโโโโโค
โ 2022-02-10 โ 904.550  โ
โโโโโโโโโโโโโโผโโโโโโโโโโโค
โ 2022-02-11 โ 860.000  โ
โโโโโโโโโโโโโโผโโโโโโโโโโโค
โ 2022-02-14 โ 875.760  โ
โโโโโโโโโโโโโโผโโโโโโโโโโโค
โ 2022-02-15 โ 922.430  โ
โโโโโโโโโโโโโโดโโโโโโโโโโโ
```
---
