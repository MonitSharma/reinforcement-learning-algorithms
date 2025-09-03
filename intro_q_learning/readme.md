### **What is RL?**

In RL, we build an agent that can make smart decisions, like an agent that learns to play a video game, or training an agent that learns to maximize its benefits by deciding on what stocks to buy and when to sell.


![alt text](rl-process.png)

Agent learns from the environment by interacting with it through trial and error and receiving rewards as unique feedback.

The goal is to maximize its expected cumulative reward. The agent's decision making process is called the policy : $\pi$

![alt text](policy.png)

Goal is to find an **optimal policy**. There are two methods to that:

1. Policy Based : Train the policy directly to learn which action to take given a state.

2. Value Based : Train a value function to learn which state is more valuable, and use this value function to take the action that leads to it.


![alt text](two-approaches.png)

#### **Value-Based Method**

We learn a value function that maps a state to the expected value of being at that state.

![alt text](vbm-1.png)

Indirectly by training a value function that outputs the value of a state or a state-action pair.

#### **Policy-Based Method**

The policy takes a state as input and outputs what action to take at that state. 