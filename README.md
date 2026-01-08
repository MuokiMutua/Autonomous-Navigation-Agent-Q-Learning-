# Autonomous Navigation Agent (Q-Learning)

<img width="1024" height="559" alt="image" src="https://github.com/user-attachments/assets/869e0976-21f8-4fad-9d83-d497b54d60c7" />


## Introduction
Unlike traditional AI that learns from static datasets, this project uses **Reinforcement Learning (RL)** to train an agent through **direct interaction** with its environment. Using the **Q-Learning algorithm**, a neon-themed robot must navigate a **5 × 5 GridWorld** to reach a goal while avoiding **lethal traps**.

---

## Objectives
- **Dynamic Pathfinding:** Train an agent to find the shortest path in a discrete environment **without prior instructions**.  
- **Exploration vs. Exploitation:** Implement an **Epsilon-Greedy strategy** to balance **discovering new routes** versus **maximizing known rewards**.  
- **Reward Optimization:** Apply the **Bellman Equation** to update the agent's memory (**Q-Table**) based on feedback from the environment.

---

## The Technology Stack
- **Framework:** Markov Decision Process (MDP)  
- **Algorithm:** Q-Learning (Off-policy Reinforcement Learning)  
- **Logic:** Bellman Equation & Temporal Difference Learning  
- **Visuals:** Seaborn Heatmaps & Matplotlib Training Curves

---

## The Process
1. **Environment Setup:** Created a **GridWorld** where:  
   - Each step costs **-1** (incentivizing speed)  
   - Falling into a pit costs **-10** (punishment)  
   - Reaching the goal rewards **+10**

2. **The Q-Table:** Initialized a **25 × 4 matrix** representing every **state-action pair** the agent may encounter.

3. **The Training Loop:** Ran **1,000 episodes**, gradually shifting the agent from **random movement** to **goal-directed behavior** as the **Epsilon value decayed**.

4. **Convergence Analysis:** Tracked **Cumulative Reward per episode** to confirm the agent successfully learned from experience.

---

## Key Insights & Results
- **Successful Convergence:** The agent reduced its average path length from **50+ random moves** to the **optimal 8 moves** within 400 episodes.  
- **Spatial Intelligence:** The **Q-Value Heatmap** shows higher values near the goal, creating a digital "gradient" that guides the agent to success.

---

## Business Applications
The logic developed can scale to real-world domains such as:  
- **Warehouse Robotics:** Optimizing paths for automated sorting robots.  
- **Autonomous Drones:** Navigating obstacles in real-time.  
- **Game AI:** Creating adaptive NPCs that respond to player behavior.
