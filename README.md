# Udacity Deep Reinforcement Learning: Continuous Control Project

## The Reacher Environment

<img src="reacher.gif"/>

In this Unity ML-Agents Reacher Environment, a double-jointed arm can move to target locations. A reward of +0.1 is provided for each step that the agent's hand is in the goal location. Thus, the goal of the agent is to maintain its position at the target location for as many time steps as possible.

The observation space consists of 33 variables corresponding to position, rotation, velocity, and angular velocities of the arm. Each action is a vector with four numbers, corresponding to torque applicable to two joints. Every entry in the action vector should be a number between -1 and 1.

### Note

The project environment contains only one agent.
The task is episodic, and in order to solve the environment, the agent must get an average score of +30 over 100 consecutive episodes.

## Deep Deterministic Policy Gradient (DDPG) Algorithm

Please see https://arxiv.org/abs/1509.02971 for the main idea of this algorithm.

The Udacity implementation of DDPG can be found at ddpg_agent.py and model.py.

Please see the Continuous Control notebook for how the DDPG Agent can be utilized for this project.

Also see Report.md
