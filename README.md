# RL for Market Making

## Overview
This project studies market making as a reinforcement learning problem and investigates whether RL agents can outperform the classical Avellaneda–Stoikov benchmark.

We implement continuous-control algorithms (PPO and SAC) to learn optimal bid-ask quoting strategies under multiple simulated market environments.

## Key Features
- Continuous action space for bid-ask spread control
- PPO and SAC as primary methods
- Benchmark comparison with Avellaneda–Stoikov model
- Multiple environments:
  - Brownian motion (baseline)
  - Jump-diffusion (stress testing)
  - Toxic order flow scenarios

## Results
- PPO and SAC demonstrate adaptive quoting behavior
- RL agents outperform the Avellaneda–Stoikov benchmark in simulated environments
- SAC shows improved robustness under noisy and non-stationary conditions

## Repository Structure
rl-market-making/
├── report/        # Final paper/report
├── notebooks/     # PPO, SAC implementations
├── src/           # Core environment and training code
├── results/       # Plots and outputs

## Installation
pip install -r requirements.txt


## Running the Code
python train.py


## Future Work
- Incorporate real limit order book data
- Risk-sensitive reward design (CVaR)
- Offline RL and execution strategies
