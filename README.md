# Swarm-RL Dynamic Lane Orchestration 🚦
**Google "Fund My Crazy" 2026 | Top 50 Build in Public Finalist**

![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)
![Stable Baselines3](https://img.shields.io/badge/Stable%20Baselines3-PPO-orange.svg)
![Pygame](https://img.shields.io/badge/Pygame-UI%20Renderer-green.svg)
![Status](https://img.shields.io/badge/Status-Prototype%20Complete-brightgreen.svg)

## 📖 The Core Concept
Urban metropolises suffer from severe asymmetric gridlock. During rush hour, inbound lanes are paralyzed while opposing lanes sit vacant. Rigid civil infrastructure relies on static painted lines, trapping cities in spatial allocations that cannot adapt to real-time traffic volumes.

**The Solution:** We abandon static paint for dynamic, edge-computed LED projections governed by decentralized Swarm Intelligence. By treating vehicles as multi-agent swarms, our Reinforcement Learning (RL) model dynamically shifts lane dividers in real-time, converting a standard `2x2` road into a `3x1` express corridor based on instant volumetric load.

## 🧠 The AI Backend (Reinforcement Learning)
The visual simulation acts as an inference engine for a Proximal Policy Optimization (PPO) neural network. 

The agent is trained in a custom `Gymnasium` environment, optimizing for maximum throughput while actively learning to penalize idle states and erratic lane toggling. 

### Telemetry Learning Curve
*The graph below demonstrates the AI's real-time decision matrix. As the inbound surge (red line) spikes, the AI autonomously shifts the active lane state to `3x1` capacity (green line) to absorb the shock, returning to `2x2` when the queue clears.*

![AI Telemetry](assets/ai_telemetry_graph.png)

## 🚀 The Digital Twin (Command Center UI)
To prove physical viability, the RL logic is translated into a high-fidelity digital twin using Pygame. 
* **Static Grid (Left):** Causes severe cumulative delay and bottlenecking during asymmetric surges.
* **Swarm-RL Grid (Right):** Dynamically shifts capacity, maintaining smooth throughput and reducing cumulative idle time by over **50%**.

*(Upload/Link your `assets/swarm_dashboard.mp4` video here in your GitHub repo)*

## 🛠️ Installation & Execution

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/YOUR_USERNAME/SwarmRL-Dynamic-Lanes.git](https://github.com/YOUR_USERNAME/SwarmRL-Dynamic-Lanes.git)
   cd SwarmRL-Dynamic-Lanes
