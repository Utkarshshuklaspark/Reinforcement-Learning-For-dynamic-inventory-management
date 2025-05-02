# 📦 Reinforcement Learning for Dynamic Inventory Management

Optimize inventory decisions using **Reinforcement Learning (RL)** to reduce holding costs, avoid stockouts, and maximize supply chain efficiency. This project uses a simulated environment to train an AI agent that learns optimal restocking strategies in a dynamic, uncertain demand scenario.

---

## 🚀 Project Overview

Inventory management is crucial in supply chain logistics. Traditional models like EOQ or (s, S) policies rely on fixed assumptions and often underperform in volatile environments.

This project applies **Reinforcement Learning** to dynamically learn and adapt inventory ordering strategies, considering:

- Variable customer demand
- Lead times
- Holding and shortage costs
- Reorder constraints

---

## 🎯 Objectives

- Formulate inventory control as a **Markov Decision Process (MDP)**
- Simulate an environment using OpenAI Gym interface
- Train a Deep Q-Network (DQN) agent to learn reorder policies
- Compare RL results with baseline (s, S) policies

---

## 🧠 Key Concepts

| Component    | Description                                               |
|--------------|-----------------------------------------------------------|
| State        | Current inventory level, pending deliveries, time step    |
| Action       | Order quantity (discrete or continuous)                   |
| Reward       | Profit - Holding cost - Shortage penalty - Ordering cost  |
| Transition   | Environment changes based on demand and agent action      |
| Policy       | Mapping from state to action (learned by agent)           |

---

## 📊 Sample Results

| Metric                  | RL Agent      | (s, S) Policy |
|-------------------------|---------------|---------------|
| Total Cost (per episode)| 1182.34       | 1543.29       |
| Avg. Stockouts          | 3.1           | 7.4           |
| Avg. Inventory Level    | 25.8 units    | 40.2 units    |

*These are simulated results. Performance may vary with parameter tuning.*

---

## 🛠️ Tech Stack

- Python 3.8+
- OpenAI Gym (custom environment)
- NumPy, Pandas
- Matplotlib / Seaborn (visualization)
- PyTorch (Deep Q-Network implementation)

---


