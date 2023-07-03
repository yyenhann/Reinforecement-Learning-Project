# Reinforecement-Learning-Project
Trading cryptocurrencies using Reinforcement Learning

Problem Statement
Trading cryptocurrencies is challenging for traders and investors to discern the best strategies for optimising their portfolios. With the ever-changing dynamics of market conditions, even the advantage of hindsight does not always reveal the most effective trading policies. In this project, we explored the use of Reinforcement Learning to train agents to automate the entire trading process and ultimately determine if a profit can be made.

Methodology and Approach
The dataset consisted of 16 cryptocurrencies with each row representing 5-minute intervals from 1st January 2022 to 19th March 2023. Features included close/open prices, high/low prices, volume, etc. The following parameters need to be defined for each environment:
State: The set of input features and variables the agent receives at timestep, t, to make a decision. This is fed into a policy (neural network) to output an action vector
Action: The output vector from the policy. The agent will execute the output action at timestep, t (e.g., buy, hold, or sell)
Weights: A transformation (mapping) of the action
Policy: A function that maps state to action (e.g., a neural network)
Reward: The reward function from taking action, at at timestep, t (e.g., the returns from taking action at)
The full dataset was split into train-validation-test in the ratio of 70-15-15. We also defined two environments - a long only environment and a long and short environment. The table summarises their comparisons:

