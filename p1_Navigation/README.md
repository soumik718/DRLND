[//]: # (Image References)

[image1]: https://user-images.githubusercontent.com/10624937/42135619-d90f2f28-7d12-11e8-8823-82b970a54d7e.gif "Trained Agent"

# Project 1: Navigation

### Project Goal
The project goal is to train a deep reinforcement learning agent to navigate a virtual world and collect as many yellow bananas as possible while avoiding blue bananas.

![Trained Agent][image1]

### Environment details

This project environment is based on [The Unity Machine Learning Agents Toolkit](https://github.com/Unity-Technologies/ml-agents)

> The Unity Machine Learning Agents Toolkit (ML-Agents) is an open-source project that enables games and simulations to serve as environments for training intelligent agents. Agents can be trained using reinforcement learning, imitation learning, neuroevolution, or other machine learning methods through a simple-to-use Python API. 

**Note:** The project environment provided by Udacity is similar to, but not identical to the [Banana Collector](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Learning-Environment-Examples.md#banana-collector) environment on the Unity ML-Agents GitHub page.

### Project Overview
For this project, you will train an agent to navigate (and collect bananas!) in a large, square world.

A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana. Thus, the goal of your agent is to collect as many yellow bananas as possible while avoiding blue bananas.

The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around the agent's forward direction. Given this information, the agent has to learn how to best select actions. Four discrete actions are available, corresponding to:

- 0 - move forward.
- 1 - move backward.
- 2 - turn left.
- 3 - turn right.

The task is episodic, and in order to solve the environment, your agent must get an average score of +13 over 100 consecutive episodes.

### Getting Started

1. Download the environment from one of the links below.  You need only select the environment that matches your operating system:
    - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux.zip)
    - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana.app.zip)
    - Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86.zip)
    - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86_64.zip)

2. Place the file in the DRLND GitHub repository, in the `p1_Navigation/` folder, and unzip (or decompress) the file. 

### Submission overview

- `Navigation.ipynb` - file with fully functional code.
- `Report.pdf` - a PDF export of the project report.
- `model.py` - the configuration of the neural network.
- Agents:

    * `dqn_agent.py` - a [DQN agent with Experience Replay and Fixed Q-Targets](https://deepmind.com/research/publications/human-level-control-through-deep-reinforcement-learning) | `checkpoint_dqn.pt` - trained agent parameters.
    * `ddqn_agent.py` - a [Double DQN agent with Experience Replay](https://arxiv.org/abs/1509.06461) | `checkpoint_ddqn.pt` - trained agent parameters.
    * `dqn_per_agent.py` - a [DQN agent with Prioritized Experience Replay](https://arxiv.org/abs/1511.05952) | `checkpoint_dqn_per.pt` - trained agent parameters.
    
- `images/` - folder contains images related to the documentation of this project.
