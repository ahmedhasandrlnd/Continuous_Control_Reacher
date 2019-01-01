# Continuous Control in Reacher Environment
Deep Reinforcement Learning Nanodegree Project 2

![Unity Reacher Continuous Control](images/reacher_continuous.gif)

## Project description
For this project, the task is to train 20 identical agents interacting within Reacher Unity environment. Each agent has a double-joined arm that can move to target locations.

* Goal: A reward of +0.1 is provided for each step that the agent's hand is in the goal location. Thus, the goal of an agent is to maintain its position at the target location for as many time steps as possible..

* The observation space consists of 33 variables corresponding to position, rotation, velocity, and angular velocities of the arm.

* Each action is a vector with four numbers, corresponding to torque applicable to two joints. Every entry in the action vector should be a number between -1 and 1.

* Solution criteria: the environment is considered as solved when the agents get an average score of +30 (over 100 consecutive episodes, and over all agents). Specifically,

	* After each episode, we add up the rewards that each agent received (without discounting), to get a score for each agent. This yields 20 (potentially different) scores. We then take the average of these 20 scores.
	* This yields an average score for each episode (where the average is over all 20 agents).

## Getting started
### Configuration
PC configuration used for this project:

* OS: Mac OS 11.3 El Capitan
* Processor: 1.3 GHz Intel Core i5
* Memory: 4GB 1600MHz DDR3
* Graphics: Intel HD Graphics 5000 1536MB

### Environment setup
For detailed Python environment setup (PyTorch, Unity Environment, and a few more Python packages) please follow these [steps](https://github.com/udacity/deep-reinforcement-learning#dependencies): 

### Structure
All project files are structured as follows:

* ddpg_agent.py - It contains agent, noise and replay buffer class implementation. agent class interacts with and learns from the environment. replay buffer class has a fixed-size buffer to store experience tuples. noise class is used to explore the environment more.
* model.py - It contains the neural network architecture for the actor and critic networks.
* checkpoint_actor.pth- It contains the trained model weights of the actor network.
* checkpoint_critic.pth- It contains the trained model weights of the critic network.
* Report.md- Explains the algorithm used and ideas for future improvement.
* README.md- It describes the project environment details, installation instruction and running code.
* images- This folder contains diiferent images used in the project.
* Reacher20.app- It contains the built in unity environment used in the project.
* Continuous_Control.ipynb- This notebook contains training code for the agent and our solution for this environment.


