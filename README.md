# Optimizing-Warehouse-Flows-with-Q-Learning
calculate optimum route in a warehouse using Q-Learning algorithm (Bellman equation)

# description
This notebook shows how to calculate the optimal route of a robot in a warehouse. The robot has to go from his location (bin A) to a target location (bin B). The algorithm uses the principle of Q-Learning to calculate the optimal sequence to reach the target.
The algorithm can then be modified to specify intermediate stops which have to be factored in. The robot must deal with these constraints while still find the optimal route.

# Q-learning algorithm
The optimization is performed using Bellman's equation which is cornerstone to the Reinforcement learning AI field.
This equation allows to calculate the value of each action as a function of future actions. The value of an action is decomposed into an immediate reward for the action (the mouvement allowing to go from one location to the next) and the discounted value of the future actions following.
As part of the learning process, the agent will iterate multiple times in the environment, allowing to recursively compute the value of all actions (the Q-Values).
These values will ultimately converge, allowing to determine the optimal route.

This is a simple case illustrating the potential behind Bellman equation. I covered a more complicated problem in this project [Minimize-Energy-consumption-with-Deep-Learning-model](https://github.com/LaurentVeyssier/Minimize-Energy-consumption-with-Deep-Learning-model) and also applied these principles to another business related situation in this [princing optimization project](https://github.com/LaurentVeyssier/Pricing-optimization-Model).

# Steps of the algorithm
- Define the environement : the states (the different possible locations here), the actions (allwoing to transit from one location to the next here), the rewards for each tuple (location x action)
- 

