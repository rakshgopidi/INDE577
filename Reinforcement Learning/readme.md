# Reinforcement Learning with Q-Learning on Taxi-v3
This code demonstrates an implementation of Q-Learning, a type of Reinforcement Learning, on the Taxi-v3 environment in OpenAI Gym.

**Environment**
The Taxi-v3 environment consists of a 5x5 grid world, where the agent (a taxi) navigates to pick up a passenger and drop them off at a specified location. The agent receives rewards and penalties depending on its actions, and the goal is to maximize the cumulative reward over time.

**Q-Learning**
Q-Learning is a model-free algorithm for learning optimal policies in a Markov Decision Process (MDP). The Q-Table represents the expected reward of taking a particular action in a given state. During training, the agent explores the environment and updates the Q-Table based on the rewards and transitions it observes. During testing, the agent follows the policy dictated by the Q-Table to make decisions.

**Implementation**
The code initializes a Q-Table with zeros, and then trains the agent for 10,000 episodes. The hyperparameters used are:

alpha: the learning rate
gamma: the discount factor
epsilon: the exploration rate
epsilon_min: the minimum exploration rate
epsilon_decay: the rate at which the exploration rate decays over time.
During training, the agent takes an action using an epsilon-greedy policy, updates the Q-Table based on the observed reward and next state, and repeats until the episode is complete.

After training, the code evaluates the agent by running 100 episodes and recording the total number of steps and penalties.

**Results**
The code prints the progress during training, and after evaluation, it prints the average number of steps and penalties per episode. Additionally, it plots the total number of penalties and timesteps per episode.