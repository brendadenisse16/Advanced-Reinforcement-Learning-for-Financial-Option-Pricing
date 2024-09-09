# Reinforcement Learning for American Options Pricing

## Overview
This project implements various Reinforcement Learning (RL) algorithms to estimate the price of American options. Specifically, we use techniques like Q-learning, Double Q-learning, Least-Squares Policy Iteration (LSPI), and Fitted Q Iteration (FQI) to solve the Optimal Stopping Problem, a challenging task in financial mathematics.

American options are a type of financial contract that gives the holder the right, but not the obligation, to buy or sell an asset at a strike price before the contract expires. This project focuses on developing RL-based methods for pricing American call and put options under the Black-Scholes model.

## Methods
The following RL algorithms are applied to estimate option prices:
1. **Q-Learning**: A reinforcement learning algorithm that estimates the optimal action-value function by iteratively updating a Q-table.
2. **Double Q-Learning**: A variant of Q-learning that reduces the overestimation bias by maintaining two Q-tables.
3. **Least-Squares Policy Iteration (LSPI)**: A batch reinforcement learning algorithm that uses least-squares temporal difference learning.
4. **Fitted Q Iteration (FQI)**: A model-free algorithm for solving control problems using function approximation.

## Black-Scholes Model
The stock price $S_t$ is modeled using a Geometric Brownian Motion under the Black-Scholes framework:

$$
dS_t = \mu S_t dt + \sigma S_t dW_t
$$

Where:
- $\mu$ is the drift (expected return rate)
- $\sigma$ is the volatility
- $W_t$ is a standard Wiener process

The aim is to simulate stock prices and apply RL techniques to determine the optimal stopping time for exercising the option.

## Project Structure
- **/main.Rmd**: RMarkdown file containing all the simulations, RL implementations, and plots.

## Setup and Installation
To run this project, follow the steps below:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/brendadenisse16/Reinforcement-Learning.git

