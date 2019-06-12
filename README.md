# DQN Report



## Introduction

This repository is the solution for the first assignment in the Udacity Deep Reinforcement Learning Nanodegree. The goal was to train an agent using DQN (Deep Q Learning) that was able to navigate sucessfuly the environment the "bananas environment" made by Unity ML Agent and collect enough rewards, represented as bananas, in order to achieve a score above a certain threshold. This is why we named our agent the "Bananahoarder". We'll by introducing the Project details.

## Project details

The following iterals contains the description of the environment

a. State

The state space consists of 37 dimensions which include yellow and blue bananas; the agent receives a reward of +1 if the agent collects a yellow banana and a reward of -1 if he collects a blue banana, otherwise the agent doesn't receive any reward. The forementioned dimensions contain the agent's velocity and the perception of objects in front of the agent.

This code trains the agent based solely in the environment obtained by unity; another posibility would be to train the agent based uniquely on the pixels produced by the image using a CNN (Convolutional Neural Network).  

b. Action spaces

There are four discrete actions available:

		- Move Forward : 0

		- Move Backwards: 1

		- Turn Left: 2

		- Turn right: 3

It is important to note that the agent doesn't act directly with the environment. A so called "brain" controls the actions within the environment and collects the information from the state. Therefore we shall call this brain the " banana brain", he went quite "bananas" after he was trained: no pun intended. 

c. Solved 

The task is episodic (it is not eternal, it ends after a while), and the environment is considered solved when the agent achieves an average score of +13 over a window of 100 consecutive episodes. 


## Getting started

a. Unity ML Agents:

First you must install the Unity toolkit. You'll find the instruction in this link, please 	      don't dispair this is probably the hardest step: <href>https://github.com/udacity/deep-reinforcement-learning#dependencies
	
b. Install
	
After you have downloaded the toolkit please install it and then download the banana's environment you can find it in the following link:  https://github.com/orangebacked/deep-reinforcement-learning/tree/master/p1_navigation . Once you have the environment.
	
c. Fun

Have fun! The implentation of the DQN has three files: model.py, dqn_agent.py, Navigation.ipynb
* model.py
-This file contained the ANN (artificial neural network) which agent finds the function that aproximates the Q table.
* dqn_agents.py
-This file creates the agent used but the reinforcement algorithm. if you wish to modify the ANN, start here.
* Navigation
-This jupyter notebook uses the two previous files and details the training process. This is the only file you need to run in order to train the agent. PLEASE DON'T LOOK AT UNITY WHILE TRAINING (it will crash and you wil have to reboot your computer and start over again, not before siting in your chair crying for half an hour).

## Instructions

Just as highlighted above if you want to train the model from scratch run the navigation jupyter notebook. Otherwise you can use the pretrained checkpoint provided in the repository.   


 
