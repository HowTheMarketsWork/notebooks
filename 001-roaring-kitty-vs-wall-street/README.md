# Episode 001: Roaring Kitty vs Wall Street: The Real GameStop Story

The video: [How The Markets Work on YouTube](https://www.youtube.com/@HowTheMarketsWork)

## What's here

**[gex_calculator.ipynb](gex_calculator.ipynb)**: a Net Gamma Exposure (GEX) calculator. It prices gamma for every strike in
an options chain with Black-Scholes, then adds it up into the one number from the video: whether dealer hedging is likely
to calm price moves (positive GEX) or speed them up (negative GEX).

Click the notebook to read it on GitHub with its outputs and chart already shown. No install needed to read it.

## Run it yourself

```bash
pip install numpy scipy matplotlib
jupyter notebook gex_calculator.ipynb
```

Then change the sample chain (strikes, open interest, volatility, days to expiry) and watch the regime flip.

## Read this first

- The options chain in the notebook is a **sample**, not live GameStop or market data.
- The sign convention (dealers long the calls and short the puts customers trade) is an **assumption**. Real dealer
  positioning is not public, and a different assumption changes the answer.
- Educational material only. Not financial, investment, legal or tax advice.
