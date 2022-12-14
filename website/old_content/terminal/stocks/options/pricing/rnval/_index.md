```
usage: rnval [-p] [-m MINI] [-M MAXI] [-r RISK] [-h]
```

Calculates the expcected value of a given option by multiplying
the payoff at each predicted stock price by the probability of
that stock price happening. This expected profit is divided by
one plus the risk free rate to determine the value of those
future dollars today. The expected payoff for each strike price
is then compared with the last traded price to determine if there
are differences in the market.

For example, if you assume the price of AAPL has an equal chance
of finishing at $100 or $200 for a given expiration, you could use
this to value an option at that expiration. To value a call with a
strike of $150, you would calculate the payoff for each stock price,
which would be $0 and $50. Then, we calculate the weighted average
payoff of $25. We need to divide this amount by the risk-free rate,
assumed to be 0.02. So the value of this option expiring in one year
is 25/1.02, or $24.51.

```
optional arguments:
  -p, --put             Show puts instead of calls (default: False)
  -m MINI, --min MINI   Minimum strike price shown (default: None)
  -M MAXI, --max MAXI   Maximum strike price shown (default: None)
  -r RISK, --risk RISK  The risk-free rate to use (default: None)
  -h, --help            show this help message (default: False)
```

Example:

```
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
