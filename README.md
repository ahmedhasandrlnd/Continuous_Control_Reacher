# Continuous Control
Deep Reinforcement Learning Nanodegree Project 2

![Unity Reacher Continuous Control](images/reacher_continuous.gif)

## Project description
For this project, the task is to train 20 identical agents interacting within Reacher Unity environment. Each agent has a double-joined arm that can move to target locations.

* Goal: A reward of +0.1 is provided for each step that the agent's hand is in the goal location. Thus, the goal of your agent is to maintain its position at the target location for as many time steps as possible..

* The observation space consists of 33 variables corresponding to position, rotation, velocity, and angular velocities of the arm.

* Each action is a vector with four numbers, corresponding to torque applicable to two joints. Every entry in the action vector should be a number between -1 and 1.

* Solution criteria: the environment is considered as solved when the agents get an average score of +30 (over 100 consecutive episodes, and over all agents). Specifically,

	* After each episode, we add up the rewards that each agent received (without discounting), to get a score for each agent. This yields 20 (potentially different) scores. We then take the average of these 20 scores.
	* This yields an average score for each episode (where the average is over all 20 agents).


