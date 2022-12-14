```
usage: blis [-l LIMIT] [-h] [--export {csv,json,xlsx}]
```

Print latest insider sales 100k. [Source: OpenInsider]

```
optional arguments:
  -l LIMIT, --limit LIMIT
                        Limit of datarows to display (default: 10)
  -h, --help            show this help message (default: False)
  --export {csv,json,xlsx}
                        Export raw data into csv, json, xlsx (default: )
```

Example:

```
2022 Feb 16, 07:48 (๐ฆ) /stocks/ins/ $ blis
                                                                               Insider Data
โโโโโณโโโโโโโโโโโโโโณโโโโโโโโโโโโโณโโโโโโโโโณโโโโโโโโโโโโโโโโโโโโโโโณโโโโโโโโโโโโโโโโโโโโโโโณโโโโโโโโโโโโโณโโโโโโโโโโโโโโณโโโโโโโโโโณโโโโโโโโโโณโโโโโโโโโโโโณโโโโโโโโโโโณโโโโโโโโโโโโโโ
โ X โ Filing Date โ Trade Date โ Ticker โ Company Name         โ Insider Name         โ Title      โ Trade Type  โ Price   โ Qty     โ Owned     โ Diff Own โ Value       โ
โกโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโฉ
โ D โ 2022-02-15  โ 2022-02-15 โ EW     โ Edwards Lifesciences โ Mussallem Michael A  โ COB, CEO   โ S - Sale+OE โ $110.09 โ -32,550 โ 3,820,007 โ -1%      โ -$3,583,289 โ
โ   โ 20:50:39    โ            โ        โ Corp                 โ                      โ            โ             โ         โ         โ           โ          โ             โ
โโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโผโโโโโโโโโโโโโโค
โ D โ 2022-02-15  โ 2022-02-11 โ AGCO   โ Agco Corp /de        โ Beck Andrew H        โ SVP, CFO   โ S - Sale+OE โ $131.83 โ -25,000 โ 107,337   โ -19%     โ -$3,295,750 โ
โ   โ 20:38:48    โ            โ        โ                      โ                      โ            โ             โ         โ         โ           โ          โ             โ
โโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโผโโโโโโโโโโโโโโค
โ D โ 2022-02-15  โ 2022-02-14 โ PUBM   โ Pubmatic, Inc.       โ Goel Amar K.         โ Chief      โ S - Sale+OE โ $29.85  โ -24,000 โ 0         โ -100%    โ -$716,444   โ
โ   โ 20:24:51    โ            โ        โ                      โ                      โ Innovation โ             โ         โ         โ           โ          โ             โ
โ   โ             โ            โ        โ                      โ                      โ Officer,   โ             โ         โ         โ           โ          โ             โ
โ   โ             โ            โ        โ                      โ                      โ 10%        โ             โ         โ         โ           โ          โ             โ
โโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโผโโโโโโโโโโโโโโค
โ D โ 2022-02-15  โ 2022-02-14 โ NET    โ Cloudflare, Inc.     โ Meresman Stanley J   โ Dir        โ S - Sale+OE โ $106.00 โ -18,622 โ 2,441     โ -88%     โ -$1,973,993 โ
โ   โ 19:57:51    โ            โ        โ                      โ                      โ            โ             โ         โ         โ           โ          โ             โ
โโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโผโโโโโโโโโโโโโโค
โ D โ 2022-02-15  โ 2022-02-14 โ AON    โ Aon Plc              โ Davies Christa       โ CFO        โ S - Sale+OE โ $283.72 โ -616    โ 200,237   โ 0%       โ -$174,772   โ
โ   โ 19:36:49    โ            โ        โ                      โ                      โ            โ             โ         โ         โ           โ          โ             โ
โโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโผโโโโโโโโโโโโโโค
โ D โ 2022-02-15  โ 2022-02-14 โ NOW    โ Servicenow, Inc.     โ Desai Chirantan      โ COO        โ S - Sale+OE โ $578.48 โ -3,000  โ 50,376    โ -6%      โ -$1,735,431 โ
โ   โ 19:05:07    โ            โ        โ                      โ Jitendra             โ            โ             โ         โ         โ           โ          โ             โ
โโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโผโโโโโโโโโโโโโโค
โ M โ 2022-02-15  โ 2022-02-11 โ IBKR   โ Interactive Brokers  โ Peterffy Thomas      โ COB        โ S - Sale    โ $73.61  โ -33,000 โ 3,874,511 โ -1%      โ -$2,429,184 โ
โ   โ 18:59:49    โ            โ        โ Group, Inc.          โ                      โ            โ             โ         โ         โ           โ          โ             โ
โโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโผโโโโโโโโโโโโโโค
โ D โ 2022-02-15  โ 2022-02-11 โ AMP    โ Ameriprise Financial โ Sweeney Joseph       โ Pres-AWM   โ S - Sale+OE โ $315.45 โ -12,981 โ 10,423    โ -55%     โ -$4,094,838 โ
โ   โ 18:10:56    โ            โ        โ Inc                  โ Edward               โ Products,  โ             โ         โ         โ           โ          โ             โ
โ   โ             โ            โ        โ                      โ                      โ Services   โ             โ         โ         โ           โ          โ             โ
โโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโผโโโโโโโโโโโโโโค
โ D โ 2022-02-15  โ 2022-02-11 โ AMP    โ Ameriprise Financial โ Thissen Karen Wilson โ EVP, GC    โ S - Sale+OE โ $313.88 โ -6,444  โ 10,472    โ -38%     โ -$2,022,661 โ
โ   โ 18:10:40    โ            โ        โ Inc                  โ                      โ            โ             โ         โ         โ           โ          โ             โ
โโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโโผโโโโโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโโผโโโโโโโโโโโโโโค
โ D โ 2022-02-15  โ 2022-02-14 โ AMP    โ Ameriprise Financial โ Truscott William F   โ CEO,       โ S - Sale+OE โ $305.09 โ -16,000 โ 28,647    โ -36%     โ -$4,881,468 โ
โ   โ 18:09:39    โ            โ        โ Inc                  โ                      โ Global     โ             โ         โ         โ           โ          โ             โ
โ   โ             โ            โ        โ                      โ                      โ Asset      โ             โ         โ         โ           โ          โ             โ
โ   โ             โ            โ        โ                      โ                      โ Management โ             โ         โ         โ           โ          โ             โ
โโโโโดโโโโโโโโโโโโโโดโโโโโโโโโโโโโดโโโโโโโโโดโโโโโโโโโโโโโโโโโโโโโโโดโโโโโโโโโโโโโโโโโโโโโโโดโโโโโโโโโโโโโดโโโโโโโโโโโโโโดโโโโโโโโโโดโโโโโโโโโโดโโโโโโโโโโโโดโโโโโโโโโโโดโโโโโโโโโโโโโโ
D: Derivative transaction in filing (usually option exercise)
M: Multiple transactions in filing; earliest reported transaction date & weighted average transaction price
```
