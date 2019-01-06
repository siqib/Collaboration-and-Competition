# Project: Collaboration and Competition


## Introduction

In this project, two agents are trained to control the rackets to bounce a ball over a net. The agent receives a reward of +0.1 if he hits the ball over the net. Otherwise if the ball hits the ground or hits out of the bouds, the agent receives a reward of -0.01. Therefore, each agent's goal is to keep the ball in play.

[//]: # (Image References)

[image1]: https://user-images.githubusercontent.com/10624937/43851024-320ba930-9aff-11e8-8493-ee547c6af349.gif "Trained Agent"
[image2]: https://user-images.githubusercontent.com/10624937/43851646-d899bf20-9b00-11e8-858c-29b5c2c94ccc.png "Crawler"

![Trained Agent][image1]

### Project Details

In the observation space, there are 8 variables corresponding to position, velocity of the ball and racket. Each agent receives its own, local observation. 

The actions space is continuous, corresponding to movement toward (or away from) the net, and jumping.

### Target of Project

The reward is received by each agent after each episode without discounting. Then we add up the scores each agent received and take a maximum of the two scores. The environment is solved when the agents get an average score of +0.5 with the maximum score over 100 consecutive episodes.


## Getting Started  


1. Download the environment from one of the links below.  You need only select the environment that matches your operating system:
    - **_Twenty (20) Agents_**
        - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Linux.zip)
        - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher.app.zip)
        - Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Windows_x86.zip)
        - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Windows_x86_64.zip)
    
   (_For Windows users_) Check out [this link](https://support.microsoft.com/en-us/help/827218/how-to-determine-whether-a-computer-is-running-a-32-bit-version-or-64) if you need help with determining if your computer is running a 32-bit version or 64-bit version of the Windows operating system.
   

   (_For AWS_) If you'd like to train the agent on AWS (and have not [enabled a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md)), then please use [this link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Linux_NoVis.zip) (version 1) or [this link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Linux_NoVis.zip) (version 2) to obtain the "headless" version of the environment.  You will **not** be able to watch the agent without enabling a virtual screen, but you will be able to train the agent.  (_To watch the agent, you should follow the instructions to [enable a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md), and then download the environment for the **Linux** operating system above._)

2. Place the file in the same folder with `Tennis.ipynb` and unzip (or decompress) the file. 


3. You would need to use the Unity ML-Agents environment in this project. Make sure you have installed [Unity ML-Agents](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Installation.md) and [NumPy](http://www.numpy.org/).

## Instructions


In the `Tennis.ipynb`, when starting the Unity ML-Agetns environment, change the `file_name` parameter to the location of your Unity Environment with `UnityEnvironment(file_name = "your path")`.   

To train the agent, simply run `Tennis.ipynb`. The trained weights of actor and critic networks are stored in files `actor_net.pth` and `critic_net.pth` respectively.



