# Project 2: Continuous Control

### Project Goal
The goal of this project is to solve the Unity ML-Agents Reacher Environment. In this environment, a double-jointed arm can move to target locations. A reward of +0.1 is provided for each step that the agent's hand is in the goal location. Thus, the goal of your agent is to maintain its position at the target location for as many time steps as possible.

<img src="https://camo.githubusercontent.com/7ad5cdff66f7229c4e9822882b3c8e57960dca4e/68747470733a2f2f73332e616d617a6f6e6177732e636f6d2f766964656f2e756461636974792d646174612e636f6d2f746f706865722f323031382f4a756e652f35623165613737385f726561636865722f726561636865722e676966">

### Project Overview
The observation space consists of 33 variables corresponding to the position, rotation, velocity, and angular velocities of the arm. Each action is a vector with four numbers, corresponding to torque applicable to two joints. Every entry in the action vector should be a number between -1 and 1. The environment is considered solved if a reward of +30 is obtained for 100 consecutive episodes.

### Algorithms
The algorithm used here is a Deep Deterministic Policy Gradient (DDPG). A DDPG is composed of two networks, actor and critic. During a step, the actor is used to estimate the best action, and the critic then uses this value as in a DDQN to evaluate the optimal action-value function.

### Submission overview

- `Continuous_Control.ipynb` - file with fully functional code.
- `Report.pdf` - a PDF export of the project report.
- `model.py` - the configuration of the neural network.
- Agents:

    * `ddpg_agent.py` - a [Deep Deterministic Policy Gradient (DDPG) Agent](https://spinningup.openai.com/en/latest/algorithms/ddpg.html)
    * `checkpoint_actor.pth` - trained actor parameters.
    * `checkpoint_critic.pth` - trained critic parameters.
    
- `images/` - folder contains images related to the documentation of 
