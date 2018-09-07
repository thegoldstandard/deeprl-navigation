# deeprl-navigation
[//]: # (Image References)

[image1]: https://user-images.githubusercontent.com/10624937/42135619-d90f2f28-7d12-11e8-8823-82b970a54d7e.gif "Trained Agent"

# Udacity Deep Reinforcement Learning (DRL) 
# Project 1: Navigation

### Introduction

This repository contains a jupyter notebook that defines and trains a DRL agent to collect bananas inside of a massive square arena. The agent is an implemenation off the Deep Q-Learning algorithm, and the game environment is a modified version of the Unity Banana Collector environment.

![Trained Agent][image1]

The agent receives a reward of +1 each time it collects collects a yellow banana and -1 each time that it collects a dark-blue banana.  The goal of the game is to collect as many yellow bananas as possible, and avoid the blue bananas, in order to maximize the final score.

The environment state space has 37 dimensions consisting of the agent's velocity and ray-based perception of the objects directly in front of the agent (is there a wall in front of the agent, is there a yellow banana in front of the agent, etc). From this information, the agent must learn how to select actions in order to maximize the stream of rewards. 

The agent can choose from four discrete actions:
- **`0`** - move forward.
- **`1`** - move backward.
- **`2`** - turn left.
- **`3`** - turn right.

The task is episodic, and is consired solved when an average score of +13 is achieved over 100 consecutive episodes.

### Getting Started

1. Install the PyTorch deep learning libary by following the instructions on the webpage:
    - [https://pytorch.org/](https://pytorch.org/)

2. Install Unity ML-Agents library by following the instructions on the webpage:
    - [https://unity3d.com/machine-learning](https://unity3d.com/machine-learning)

3. Download the custom Udacity-Unity environment from one of the links below.  You need only select the environment that matches your operating system:
    - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux.zip)
    - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana.app.zip)
    - Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86.zip)
    - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86_64.zip)
    
    (_For Windows users_) Check out [this link](https://support.microsoft.com/en-us/help/827218/how-to-determine-whether-a-computer-is-running-a-32-bit-version-or-64) if you need help with determining if your computer is running a 32-bit version or 64-bit version of the Windows operating system.

    (_For AWS_) If you'd like to train the agent on AWS (and have not [enabled a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md)), then please use [this link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux_NoVis.zip) to obtain the environment.

4. Place the file in the cloned Github repository and unzip (or decompress) the file. 

### Instructions

Open and run the Jupyter notebook titled: `Report.ipynb` to train the DRL agent. 

