# Project 1 - Navigation

Project description
=========
For this project, I implemented a navigation system to guide the agent to capture yello bananas and avoid blue bananas. Here are some descriptions of the agent from Udacity project introduction. 

A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana. Thus, the goal of your agent is to collect as many yellow bananas as possible while avoiding blue bananas.

The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around the agent's forward direction. Given this information, the agent has to learn how to best select actions. Four discrete actions are available, corresponding to:

- 0 - move forward
- 1 - move backward
- 2 - turn left
- 3 - turn right

The task is episodic, and in order to solve the environment, your agent must get an average score of +13 over 100 consecutive episodes.

Getting Started
=========
1. Setting up the enviroment. There are different ways to implement the training environmenent. I used the workspace hosted in Udacity directly. All the required python libraries including Pytorch with GPU supported are installed which is very easy to use. If you are not able to use that development environment, you can clone the [DRLND](https://github.com/udacity/deep-reinforcement-learning#dependencies) from GitHub and install the required libraries. 

2. Install required libraries. 

```
pip install -r requirements.txt
```

3. Implement dqn_agent.py and model.py. The DQN and double DQN models are implemented through these two files. 

4. Start training in Navigation.ipynb notebook. The code in the notebook is pretty self-explanatory. I implemented two models and their performances are compared using line charts. 

Description
==========
- dqn_agent.py: code for the agent
- model.py: code for deep neural network
- simple_dqn.pth: saved model for simple DQN model
- double_dqn.pth: saved model for double DQN model
- Navigation.ipynb: notebook containing the code for training. 


Instructions
==========
Execute the code in Navigation.ipynb to reproduce the training process

Results
==========

1. The simple DQN reached target score in episode 439. 
2. The double DQN reached target score in episode 400. 
3. The plots of score vs episode are ploted as below.


![simple DQN]('https://github.com/larui529/UdacityDeepReinforcementLearning/blob/master/Navigator/imgs/simple_dqn.JPG')
![double DQN]('https://github.com/larui529/UdacityDeepReinforcementLearning/blob/master/Navigator/imgs/double_dqn.JPG')

Future Work
========
1. Implement DQN algorithm using pixels.
2. Implement Dueling network for Deep Reinforcement Learning.
