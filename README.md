HMM Regime-Switching Portfolio Allocation
A dynamic multi-asset allocation system that detects hidden market regimes using Hidden Markov Models and shifts capital across equities, bonds, and safe havens using walk-forward validation.

Overview
Static portfolios like 60/40 often break down during market regime shifts. This project builds a regime-aware engine that classifies latent states, adapts portfolio objectives by regime, and evaluates performance under realistic transaction costs.

Features
HMM-based regime detection.

Regime mapping into Bull, Bear, and Crisis states.

Dynamic portfolio optimization.

Walk-forward validation to avoid look-ahead bias.

Turnover and transaction cost modeling.

Benchmark comparison against 60/40 and equal-weight portfolios.

Performance tear sheet with standard risk-adjusted metrics.

Tech Stack
Python 3.9+

NumPy

Pandas

yfinance

hmmlearn

CVXPY

SciPy

Matplotlib

Data Sources
Yahoo Finance for asset prices.

CBOE VIX as a volatility proxy.

Optional macro indicators for future extension.

Pipeline
Download and clean market data.

Engineer rolling features.

Fit an HMM to detect regimes.

Map each regime to a portfolio objective.

Run walk-forward backtests.

Compare against static benchmarks.

Export tear sheets and charts.

Outputs
Trained HMM model.

Regime labels overlaid on price history.

Transition probability matrix.

Dynamic allocation backtest.

Equity curve and regime charts.

Performance tear sheet CSV.

Weight and turnover history CSV.


