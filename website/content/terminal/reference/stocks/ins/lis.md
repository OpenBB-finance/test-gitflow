---
title: lis
description: OpenBB Terminal Function
---

# lis

Print latest insider sales. [Source: OpenInsider]

### Usage

```python
lis [-l LIMIT]
```

---

## Parameters

| Name | Description | Default | Optional | Choices |
| ---- | ----------- | ------- | -------- | ------- |
| limit | Limit of datarows to display | 10 | True | None |


---

## Examples

```python
2022 Feb 16, 07:56 (๐ฆ) /stocks/ins/ $ lis
                                                                               Insider Data
โโโโโณโโโโโโโโโโโโโโณโโโโโโโโโโโโโณโโโโโโโโโณโโโโโโโโโโโโโโโโโโโโโโโณโโโโโโโโโโโโโโโโโโโโโโณโโโโโโโโโโโโโณโโโโโโโโโโโโโโณโโโโโโโโโโณโโโโโโโโโโณโโโโโโโโโโโโณโโโโโโโโโโโณโโโโโโโโโโโโโโ
โ X โ Filing Date โ Trade Date โ Ticker โ Company Name         โ Insider Name        โ Title      โ Trade Type  โ Price   โ Qty     โ Owned     โ Diff Own โ Value       โ
โกโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโฉ
โ D โ 2022-02-15  โ 2022-02-14 โ BVS    โ Bioventus Inc.       โ D'Adamio Anthony    โ SVP, GC    โ S - Sale+OE โ $11.99  โ -1,294  โ 18,672    โ -6%      โ -$15,513    โ
โ   โ 21:31:03    โ            โ        โ                      โ                     โ            โ             โ         โ         โ           โ          โ             โ
โโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโผโโโโโโโโโโโโโโค
โ D โ 2022-02-15  โ 2022-02-14 โ BVS    โ Bioventus Inc.       โ Anglum Gregory O.   โ SVP, CFO   โ S - Sale+OE โ $11.99  โ -1,294  โ 55,013    โ -2%      โ -$15,518    โ
โ   โ 21:27:43    โ            โ        โ                      โ                     โ            โ             โ         โ         โ           โ          โ             โ
โโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโผโโโโโโโโโโโโโโค
โ D โ 2022-02-15  โ 2022-02-14 โ BVS    โ Bioventus Inc.       โ Nosenzo John        โ Chief      โ S - Sale+OE โ $11.99  โ -534    โ 43,370    โ -1%      โ -$6,401     โ
โ   โ 21:17:44    โ            โ        โ                      โ                     โ Commercial โ             โ         โ         โ           โ          โ             โ
โ   โ             โ            โ        โ                      โ                     โ Officer    โ             โ         โ         โ           โ          โ             โ
โโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโผโโโโโโโโโโโโโโค
โ D โ 2022-02-15  โ 2022-02-11 โ PGNY   โ Progyny, Inc.        โ Schlanger David J   โ Exec COB   โ S - Sale+OE โ $42.00  โ -1,000  โ 84,000    โ -1%      โ -$42,000    โ
โ   โ 21:09:05    โ            โ        โ                      โ                     โ            โ             โ         โ         โ           โ          โ             โ
โโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโผโโโโโโโโโโโโโโค
โ D โ 2022-02-15  โ 2022-02-15 โ EW     โ Edwards Lifesciences โ Mussallem Michael A โ COB, CEO   โ S - Sale+OE โ $110.09 โ -32,550 โ 3,820,007 โ -1%      โ -$3,583,289 โ
โ   โ 20:50:39    โ            โ        โ Corp                 โ                     โ            โ             โ         โ         โ           โ          โ             โ
โโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโผโโโโโโโโโโโโโโค
โ D โ 2022-02-15  โ 2022-02-11 โ AGCO   โ Agco Corp /de        โ Beck Andrew H       โ SVP, CFO   โ S - Sale+OE โ $131.83 โ -25,000 โ 107,337   โ -19%     โ -$3,295,750 โ
โ   โ 20:38:48    โ            โ        โ                      โ                     โ            โ             โ         โ         โ           โ          โ             โ
โโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโผโโโโโโโโโโโโโโค
โ D โ 2022-02-15  โ 2022-02-14 โ PUBM   โ Pubmatic, Inc.       โ Goel Amar K.        โ Chief      โ S - Sale+OE โ $29.85  โ -24,000 โ 0         โ -100%    โ -$716,444   โ
โ   โ 20:24:51    โ            โ        โ                      โ                     โ Innovation โ             โ         โ         โ           โ          โ             โ
โ   โ             โ            โ        โ                      โ                     โ Officer,   โ             โ         โ         โ           โ          โ             โ
โ   โ             โ            โ        โ                      โ                     โ 10%        โ             โ         โ         โ           โ          โ             โ
โโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโผโโโโโโโโโโโโโโค
โ D โ 2022-02-15  โ 2022-02-14 โ NET    โ Cloudflare, Inc.     โ Meresman Stanley J  โ Dir        โ S - Sale+OE โ $106.00 โ -18,622 โ 2,441     โ -88%     โ -$1,973,993 โ
โ   โ 19:57:51    โ            โ        โ                      โ                     โ            โ             โ         โ         โ           โ          โ             โ
โโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโผโโโโโโโโโโโโโโค
โ D โ 2022-02-15  โ 2022-02-14 โ AON    โ Aon Plc              โ Davies Christa      โ CFO        โ S - Sale+OE โ $283.72 โ -616    โ 200,237   โ 0%       โ -$174,772   โ
โ   โ 19:36:49    โ            โ        โ                      โ                     โ            โ             โ         โ         โ           โ          โ             โ
โโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโผโโโโโโโโโโโโโโค
โ D โ 2022-02-15  โ 2022-02-15 โ RYTM   โ Rhythm               โ Shulman Joseph      โ Chief      โ S - Sale+OE โ $6.10   โ -557    โ 1,006     โ -36%     โ -$3,398     โ
โ   โ 19:32:08    โ            โ        โ Pharmaceuticals,     โ                     โ Technical  โ             โ         โ         โ           โ          โ             โ
โ   โ             โ            โ        โ Inc.                 โ                     โ Officer    โ             โ         โ         โ           โ          โ             โ
โโโโโดโโโโโโโโโโโโโโดโโโโโโโโโโโโโดโโโโโโโโโดโโโโโโโโโโโโโโโโโโโโโโโดโโโโโโโโโโโโโโโโโโโโโโดโโโโโโโโโโโโโดโโโโโโโโโโโโโโดโโโโโโโโโโดโโโโโโโโโโดโโโโโโโโโโโโดโโโโโโโโโโโดโโโโโโโโโโโโโโ
D: Derivative transaction in filing (usually option exercise)
```
---
