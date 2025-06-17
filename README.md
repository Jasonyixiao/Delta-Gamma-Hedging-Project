# Black–Scholes Delta–Gamma Hedging Simulation

## Overview
This project implements a self-financing delta and delta–gamma hedging strategy for a short European call under the Black–Scholes framework. It models the underlying asset dynamics with drift-infused geometric Brownian motion and uses Monte Carlo simulation to quantify P&L distributions, variance reduction, and tail-risk improvements.

## Features
- **Drift-Infused GBM**: Simulates stock paths using geometric Brownian motion with configurable drift and volatility.
- **Hedging Strategies**: Implements both delta-only and delta–gamma hedges.
- **Self-Financing**: Ensures all trades are funded from initial call proceeds with no external cash flows.
- **Constraints**: Incorporates integer-quantity trading and transaction costs.
- **Monte Carlo Engine**: Runs large-scale simulations across varying parameters to generate P&L statistics.
- 
## Methodology

- **Hedging Setup**: Short one call position; initial hedge created using call proceeds.

- **Rebalancing**: At each timestep, update hedge positions to neutralize delta and gamma.

- **Self-Financing**: Ensure all rebalancing trades draw from portfolio value.

- **Simulation**: Generate 1M correlated GBM paths to evaluate P&L metrics.

## Results

1. Delta–gamma hedging reduces P&L variance by ~30% compared to delta-only hedging.

2. Tail-risk (10th percentile loss) is significantly improved under the delta–gamma strategy.
