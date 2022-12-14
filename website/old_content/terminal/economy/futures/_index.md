```
usage: futures [-c {energy,metals,meats,grains,softs}] [-s {ticker,last,change,prevClose}] [-a] [-h] [--export {csv,json,xlsx}]
```

Futures/Commodities frrom Wall St. Journal and FinViz.

```
optional arguments:
  -c {energy,metals,meats,grains,softs}, --commodity {energy,metals,meats,grains,softs}
                         Obtain commodity futures from FinViz (default: )
  -s {ticker,last,change,prevClose}, --sortby {ticker,last,change,prevClose}
  -r, --reverse          Data is sorted in descending order by default.
                         Reverse flag will sort it in an ascending way.
                         Only works when raw data is show this help message (default: False)
  --export {csv,json,xlsx}
                         Export raw data into csv, json, xlsx (default: )
```

Example:

```
2022 Mar 15, 07:02 (๐ฆ) /economy/ $ futures
     Futures/Commodities [Source: Wall St. Journal]
โโโโโโโโโโโโโโโโโโโโโโโโโโโโโณโโโโโโโโโโณโโโโโโโโโโณโโโโโโโโ
โ                           โ Price   โ Chg     โ %Chg  โ
โกโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโฉ
โ Crude Oil Futures         โ 97.11   โ -5.90   โ -5.73 โ
โโโโโโโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโค
โ Brent Crude Futures       โ 101.01  โ -5.89   โ -5.51 โ
โโโโโโโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโค
โ Gold Futures              โ 1930.50 โ -30.30  โ -1.55 โ
โโโโโโโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโค
โ Silver Futures            โ 24.875  โ -0.423  โ -1.67 โ
โโโโโโโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโค
โ Natural Gas Futures       โ 4.601   โ -0.101  โ -2.15 โ
โโโโโโโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโค
โ Unleaded Gasoline Futures โ 3.0197  โ -0.1492 โ -4.71 โ
โโโโโโโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโค
โ Copper Futures            โ 4.5005  โ -0.0225 โ -0.50 โ
โโโโโโโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโค
โ Corn Futures              โ 739.00  โ -9.25   โ -1.24 โ
โโโโโโโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโค
โ Wheat Futures             โ 1126.50 โ 30.25   โ 2.76  โ
โโโโโโโโโโโโโโโโโโโโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโค
โ Bloomberg Commodity Index โ 121.16  โ -2.64   โ -2.13 โ
โโโโโโโโโโโโโโโโโโโโโโโโโโโโโดโโโโโโโโโโดโโโโโโโโโโดโโโโโโโโ

2022 Mar 15, 07:03 (๐ฆ) /economy/ $ futures energy
            Future Table [Source: FinViz]
โโโโโโโโโโโโโโโโโโโณโโโโโโโโโโโโณโโโโโโโโโณโโโโโโโโโโโโโ
โ                 โ prevClose โ last   โ change (%) โ
โกโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโฉ
โ Ethanol         โ 2.16      โ 2.22   โ 2.78       โ
โโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโโโค
โ Gasoline RBOB   โ 3.17      โ 3.02   โ -4.82      โ
โโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโโโค
โ Crude Oil Brent โ 106.90    โ 101.01 โ -5.51      โ
โโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโโโค
โ Natural Gas     โ 4.66      โ 4.56   โ -2.10      โ
โโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโโโค
โ Heating Oil     โ 3.28      โ 3.07   โ -6.44      โ
โโโโโโโโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโโโค
โ Crude Oil WTI   โ 103.01    โ 97.14  โ -5.70      โ
โโโโโโโโโโโโโโโโโโโดโโโโโโโโโโโโดโโโโโโโโโดโโโโโโโโโโโโโ

2022 Mar 15, 07:04 (๐ฆ) /economy/ $ futures metals
         Future Table [Source: FinViz]
โโโโโโโโโโโโโณโโโโโโโโโโโโณโโโโโโโโโโณโโโโโโโโโโโโโ
โ           โ prevClose โ last    โ change (%) โ
โกโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโฉ
โ Silver    โ 25.30     โ 24.88   โ -1.65      โ
โโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโโโโค
โ Platinum  โ 1052.30   โ 1021.50 โ -2.93      โ
โโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโโโโค
โ Palladium โ 2417.60   โ 2450.50 โ 1.36       โ
โโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโโโโค
โ Copper    โ 4.52      โ 4.49    โ -0.64      โ
โโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโโโโค
โ Gold      โ 1960.80   โ 1930.30 โ -1.56      โ
โโโโโโโโโโโโโดโโโโโโโโโโโโดโโโโโโโโโโดโโโโโโโโโโโโโ

2022 Mar 15, 07:04 (๐ฆ) /economy/ $ futures meats
           Future Table [Source: FinViz]
โโโโโโโโโโโโโโโโโณโโโโโโโโโโโโณโโโโโโโโโณโโโโโโโโโโโโโ
โ               โ prevClose โ last   โ change (%) โ
โกโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโฉ
โ Lean Hogs     โ 102.72    โ 102.17 โ -0.54      โ
โโโโโโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโโโค
โ Live Cattle   โ 137.30    โ 140.35 โ 2.22       โ
โโโโโโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโผโโโโโโโโโโโโโค
โ Feeder Cattle โ 157.97    โ 162.43 โ 2.82       โ
โโโโโโโโโโโโโโโโโดโโโโโโโโโโโโดโโโโโโโโโดโโโโโโโโโโโโโ

2022 Mar 15, 07:04 (๐ฆ) /economy/ $ futures grains
           Future Table [Source: FinViz]
โโโโโโโโโโโโโโโโณโโโโโโโโโโโโณโโโโโโโโโโณโโโโโโโโโโโโโ
โ              โ prevClose โ last    โ change (%) โ
โกโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโฉ
โ Wheat        โ 1096.25   โ 1127.50 โ 2.85       โ
โโโโโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโโโโค
โ Soybeans     โ 1670.50   โ 1646.00 โ -1.47      โ
โโโโโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโโโโค
โ Rough Rice   โ 16.10     โ 16.14   โ 0.25       โ
โโโโโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโโโโค
โ Oats         โ 662.00    โ 653.75  โ -1.25      โ
โโโโโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโโโโค
โ Soybean Meal โ 484.30    โ 476.40  โ -1.63      โ
โโโโโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโโโโค
โ Soybean oil  โ 73.95     โ 72.90   โ -1.42      โ
โโโโโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโโโโค
โ Corn         โ 748.25    โ 739.75  โ -1.14      โ
โโโโโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโโโโค
โ Canola       โ 1139.10   โ 1113.40 โ -2.26      โ
โโโโโโโโโโโโโโโโดโโโโโโโโโโโโดโโโโโโโโโโดโโโโโโโโโโโโโ

2022 Mar 15, 07:04 (๐ฆ) /economy/ $ futures softs
           Future Table [Source: FinViz]
โโโโโโโโโโโโโโโโณโโโโโโโโโโโโณโโโโโโโโโโณโโโโโโโโโโโโโ
โ              โ prevClose โ last    โ change (%) โ
โกโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโโฉ
โ Sugar        โ 19.13     โ 18.74   โ -2.04      โ
โโโโโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโโโโค
โ Lumber       โ 1159.20   โ 1104.00 โ -4.76      โ
โโโโโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโโโโค
โ Coffee       โ 218.80    โ 215.05  โ -1.71      โ
โโโโโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโโโโค
โ Orange Juice โ 138.70    โ 142.00  โ 2.38       โ
โโโโโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโโโโค
โ Cotton       โ 118.77    โ 118.06  โ -0.60      โ
โโโโโโโโโโโโโโโโผโโโโโโโโโโโโผโโโโโโโโโโผโโโโโโโโโโโโโค
โ Cocoa        โ 2611.00   โ 2556.00 โ -2.11      โ
โโโโโโโโโโโโโโโโดโโโโโโโโโโโโดโโโโโโโโโโดโโโโโโโโโโโโโ
```
