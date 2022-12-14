---
title: lit
description: OpenBB Terminal Function
---

# lit

Print latest insider trading. [Source: OpenInsider]

### Usage

```python
lit [-l LIMIT]
```

---

## Parameters

| Name | Description | Default | Optional | Choices |
| ---- | ----------- | ------- | -------- | ------- |
| limit | Limit of datarows to display | 10 | True | None |


---

## Examples

```python
2022 Feb 16, 07:58 (๐ฆ) /stocks/ins/ $ lit
                                                                                Insider Data
โโโโโโณโโโโโโโโโโโโโโณโโโโโโโโโโโโโณโโโโโโโโโณโโโโโโโโโโโโโโโโโโโโณโโโโโโโโโโโโโโโโโโโโโโโณโโโโโโโโโโโโโณโโโโโโโโโโโโโโโณโโโโโโโโโณโโโโโโโโโโโโโณโโโโโโโโโโโโณโโโโโโโโโโโณโโโโโโโโโโโโโโโ
โ X  โ Filing Date โ Trade Date โ Ticker โ Company Name      โ Insider Name         โ Title      โ Trade Type   โ Price  โ Qty        โ Owned     โ Diff Own โ Value        โ
โกโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโฉ
โ M  โ 2022-02-16  โ 2022-02-09 โ ZIVO   โ Zivo Bioscience,  โ Maggiore Christopher โ Dir, 10%   โ P - Purchase โ $3.72  โ +91,334    โ 803,105   โ +13%     โ +$340,098    โ
โ    โ 06:02:09    โ            โ        โ Inc.              โ D.                   โ            โ              โ        โ            โ           โ          โ              โ
โโโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโผโโโโโโโโโโโโโโโค
โ M  โ 2022-02-15  โ 2022-02-11 โ RSVR   โ Reservoir Media,  โ Richmond Hill        โ May be     โ P - Purchase โ $6.75  โ +136,364   โ 136,364   โ New      โ +$920,717    โ
โ    โ 21:57:01    โ            โ        โ Inc.              โ Investments, LLC     โ deemed a   โ              โ        โ            โ           โ          โ              โ
โ    โ             โ            โ        โ                   โ                      โ 10% owner  โ              โ        โ            โ           โ          โ              โ
โโโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโผโโโโโโโโโโโโโโโค
โ M  โ 2022-02-15  โ 2022-02-11 โ RSVR   โ Reservoir Media,  โ Richmond Hill        โ May be     โ P - Purchase โ $6.75  โ +58,441    โ 58,441    โ New      โ +$394,588    โ
โ    โ 21:56:17    โ            โ        โ Inc.              โ Capital Partners, LP โ deemed a   โ              โ        โ            โ           โ          โ              โ
โ    โ             โ            โ        โ                   โ                      โ 10% owner  โ              โ        โ            โ           โ          โ              โ
โโโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโผโโโโโโโโโโโโโโโค
โ M  โ 2022-02-15  โ 2022-02-11 โ KNTE   โ Kinnate Biopharma โ Gordon Carl L        โ Dir        โ P - Purchase โ $10.17 โ +195,700   โ 4,043,629 โ +5%      โ +$1,989,446  โ
โ    โ 21:51:12    โ            โ        โ Inc.              โ                      โ            โ              โ        โ            โ           โ          โ              โ
โโโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโผโโโโโโโโโโโโโโโค
โ M  โ 2022-02-15  โ 2022-02-11 โ KNTE   โ Kinnate Biopharma โ Orbimed Advisors LLC โ Dir        โ P - Purchase โ $10.17 โ +195,700   โ 4,043,629 โ +5%      โ +$1,989,446  โ
โ    โ 21:42:44    โ            โ        โ Inc.              โ                      โ            โ              โ        โ            โ           โ          โ              โ
โโโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโผโโโโโโโโโโโโโโโค
โ DM โ 2022-02-15  โ 2022-02-14 โ RSVR   โ Reservoir Media,  โ Cook Stephen M.      โ Dir        โ P - Purchase โ $7.29  โ +41,510    โ 1,057,171 โ +4%      โ +$302,565    โ
โ    โ 21:32:18    โ            โ        โ Inc.              โ                      โ            โ              โ        โ            โ           โ          โ              โ
โโโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโผโโโโโโโโโโโโโโโค
โ D  โ 2022-02-15  โ 2022-02-14 โ BVS    โ Bioventus Inc.    โ D'Adamio Anthony     โ SVP, GC    โ S - Sale+OE  โ $11.99 โ -1,294     โ 18,672    โ -6%      โ -$15,513     โ
โ    โ 21:31:03    โ            โ        โ                   โ                      โ            โ              โ        โ            โ           โ          โ              โ
โโโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโผโโโโโโโโโโโโโโโค
โ DM โ 2022-02-15  โ 2022-02-11 โ AREN   โ Arena Group       โ B. Riley Financial,  โ 10%        โ P - Purchase โ $8.26  โ +1,977,982 โ 5,411,514 โ +58%     โ +$16,329,921 โ
โ    โ 21:30:53    โ            โ        โ Holdings, Inc.    โ Inc.                 โ            โ              โ        โ            โ           โ          โ              โ
โโโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโผโโโโโโโโโโโโโโโค
โ D  โ 2022-02-15  โ 2022-02-14 โ BVS    โ Bioventus Inc.    โ Anglum Gregory O.    โ SVP, CFO   โ S - Sale+OE  โ $11.99 โ -1,294     โ 55,013    โ -2%      โ -$15,518     โ
โ    โ 21:27:43    โ            โ        โ                   โ                      โ            โ              โ        โ            โ           โ          โ              โ
โโโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโผโโโโโโโโโโโโโโโค
โ D  โ 2022-02-15  โ 2022-02-14 โ BVS    โ Bioventus Inc.    โ Nosenzo John         โ Chief      โ S - Sale+OE  โ $11.99 โ -534       โ 43,370    โ -1%      โ -$6,401      โ
โ    โ 21:17:44    โ            โ        โ                   โ                      โ Commercial โ              โ        โ            โ           โ          โ              โ
โ    โ             โ            โ        โ                   โ                      โ Officer    โ              โ        โ            โ           โ          โ              โ
โโโโโโดโโโโโโโโโโโโโโดโโโโโโโโโโโโโดโโโโโโโโโดโโโโโโโโโโโโโโโโโโโโดโโโโโโโโโโโโโโโโโโโโโโโดโโโโโโโโโโโโโดโโโโโโโโโโโโโโโดโโโโโโโโโดโโโโโโโโโโโโโดโโโโโโโโโโโโดโโโโโโโโโโโดโโโโโโโโโโโโโโโ
D: Derivative transaction in filing (usually option exercise)
M: Multiple transactions in filing; earliest reported transaction date & weighted average transaction price
```
---
