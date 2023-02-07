# ReinforcementLearning

## K-Armed Bandit
Agent who chooses between $k$ actions, receives rewards  based on the choosen action. The goal is to maximize the expected reward. 

First version of K-Armed Bandit is **Random Agent**, where he chooses arms randomly. So the $q$ estimated is changing at each arm because Agent always explore.

Next option is **$\epsilon$-greedy Agent** where Agent choose between exploration and exploitation.
We choose the probability $\epsilon$ of exploration. So the probability of exploitation is $1-\epsilon$.
When Agent choose random number smaller that $\epsilon$ he explore, otherwise he exploit the best arm.

**Optimistic Agent** at the begining has big value at each arm. He chooses the best arm at each iteration so the values becomes smaller and smaller, but at the same time he explore many arms.

**Upper Confidence Bound Agent** chooses the best $q$ optimistic value. This value is created based on the $q$ estimated value, exploration parameter, number of steps and number of times when this arm was choosen.

## Dynamic Programming
Agent is in the labyrinth. Every step he takes, he gets negative reward. Moreover, at each place he gets reward associated with this state. The clue of the problem is to find the best way to exit. He chooses the best policy to get less pushment score.


## Monte Carlo for Black Jack
Agent remembers all states and actions. He gets reward if he win and pushment when he loss. At each step he use determined policy decide if he hit or draw and learns new policy based on the statistic of number of win and loss. 

## Q-Learning in Cliff Walking Environment
Agent has to get from the start to exit of the grid, but there is cliff so when he gets to the cliff he drops he get high punishment and has to start walking from the start. At each step he gets $-1$ punishment so he wants to get as fast as he can, avoiding the cliff. 

## Linear Regression
The clue is to find the best linear function which describe model. We used cost function and the goal is to minimize the cost. The best model will be found using gradient descent. We should continue algorithm until the cost stops decreasing.
