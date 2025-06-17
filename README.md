# Black–Scholes Delta–Gamma Hedging Simulation

## Overview
This project implements a self-financing delta and delta–gamma hedging strategy for a short European call under the Black–Scholes framework. It models the underlying asset dynamics with drift-infused geometric Brownian motion and uses Monte Carlo simulation to quantify P&L distributions, variance reduction, and tail-risk improvements.

## Features
- **Drift-Infused GBM**: Simulates stock paths using geometric Brownian motion with configurable drift and volatility.
- **Hedging Strategies**: Implements both delta-only and delta–gamma hedges.
- **Self-Financing**: Ensures all trades are funded from initial call proceeds with no external cash flows.
- **Constraints**: Incorporates integer-quantity trading and transaction costs.
- **Monte Carlo Engine**: Runs large-scale simulations across varying parameters to generate P&L statistics.
