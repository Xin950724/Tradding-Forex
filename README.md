
Technical indicators and overlays to run technical analysis with JavaScript / TypeScript.

## Motivation

The "trading-signals" library provides a TypeScript implementation for common technical indicators with arbitrary-precision decimal arithmetic.

The main focus of this library is on the accuracy of calculations, but using the provided [faster implementations][2] you can also use it where performance is important.

All indicators can be updated over time by streaming data (prices or candles) to the `update` method. Some indicators also provide `static` batch methods for further performance improvements when providing data up-front during a backtest or historical data import.

## Benefits & Features

- **Accurate.** Indicators with intervals will return a result only when the period is reached.
- **Convenient.** Indicators with intervals will save their all-time highs and lows.
- **Fast.** If you need high throughput, you can use the included [faster implementations][2].
- **Flexible.** All advanced indicators support different smoothing overlays (WSMA, etc.).
- **Modern.** Uses ECMAScript Modules (ESM) syntax.
- **Precise.** Better accuracy than calculating with primitive numbers thanks to [big.js][1].
- **Robust.** Checked against common division by zero mistakes.
- **Tested.** Code coverage is 100%. No surprises when using it.
- **Typed.** Source code is 100% TypeScript. No need to install external typings.
- **Verified.** All results are verified with [other libraries](#alternatives) to guarantee correctness.
- **Versatile.** Indicators can be updated up-front or by streaming prices.

## Technical Indicator Types

- Trend indicators: Measure the direction of a trend (uptrend, downtrend or sideways trend)
- Volume indicators: Measure the strength of a trend (based on volume)
- Volatility indicators: Measure how much disagreement there is in the market based on price (statistical measure of its dispersion)
- Momentum indicators: Measure the strength of a trend (based on price / speed of price movement)

## Supported Technical Indicators

1. Acceleration Bands (ABANDS)
1. Accelerator Oscillator (AC)
1. Average Directional Index (ADX)
1. Average True Range (ATR)
1. Awesome Oscillator (AO)
1. Bollinger Bands (BBANDS)
1. Bollinger Bands Width (BBW)
1. Center of Gravity (CG)
1. Commodity Channel Index (CCI)
1. Directional Movement Index (DMI / DX)
1. Double Exponential Moving Average (DEMA)
1. Dual Moving Average (DMA)
1. Exponential Moving Average (EMA)
1. Mean Absolute Deviation (MAD)
1. Momentum (MOM / MTM)
1. Moving Average Convergence Divergence (MACD)
1. On-Balance Volume (OBV)
1. Rate-of-Change (ROC)
1. Relative Strength Index (RSI)
1. Simple Moving Average (SMA)
1. Stochastic Oscillator (STOCH)
1. Stochastic RSI (STOCHRSI)
1. True Range (TR)
1. Wilder's Smoothed Moving Average (WSMA / WMA / WWS / SMMA / MEMA)

Utility Methods:

1. Average / Mean
1. Standard Deviation
1. Rolling Standard Deviation


