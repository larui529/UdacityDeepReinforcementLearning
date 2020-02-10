# Project: Continuous Control

Description
=========================
For this project, we trained a double-jointed arm agent to follow a target location.

Problem Statement
===========================
In this environment, a double-jointed arm can move to target locations. A reward of +0.1 is provided for each step that the agent's hand is in the goal location. Thus, the goal of your agent is to maintain its position at the target location for as many time steps as possible.

The observation space consists of 33 variables corresponding to position, rotation, velocity, and angular velocities of the arm. Each action is a vector with four numbers, corresponding to torque applicable to two joints. Every entry in the action vector should be a number between -1 and 1.

The task is episodic, with 1000 timesteps per episode. In order to solve the environment, the agent must get an average score of +30 over 100 consecutive episodes.

Files
===============
- Continuous_Control.ipynb: Notebook used to control and train the agent
- ddpg_agent.py: Create an Agent class that interacts with and learns from the environment
- model.py: Actor and Citric classes
- report.pdf: Technical report

Environment Option
===============
There are two versions of the environment to select:

## Option 1: Solve the first version
The task is episodic, and in order to solve the environment, your agent must get an average score of +30 over 100 consecutive episodes.

## Option2: Solve the second version
The barrier for solving the second version of the environment is slightly different, to take into account the presence of many agents. In particular, your agents must get an average score of +30 (over 100 consecutive episodes, and over all agents). 

I chose the option 2 during training


Dependencies
==============
The training job was done on a AWS ec2 instance. The instance used ubuntu 18.84 system and with tensorflow and mxnet pre-installed. 

To install other dependencies. Follow [this](https://github.com/udacity/deep-reinforcement-learning#dependencies) instruction to activate conda environment clone the github repository.

under the ~/deep-reinforcement-learning/python/ input the following command:

```
pip install requirements.txt
```

Futhermore, you need to download the environment from the link below. The ec2 instance doesn't support visualization of agent. So I used *Reacher_Linux_NoVis* agent.


AWS EC2: [link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Linux_NoVis.zip)

Running 
==============
Run the cells in the notebook Continuous_control.ipynb to train an agent that solves our required task of moving the double-jointed arm. 