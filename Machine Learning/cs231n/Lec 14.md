# Deep Reinforcement Learning
## Reinforcement Learning
> Problems involving an agent interacting with an environment, which provides numeric reward signals
* Goal : Learn how to take actions in order to maximize reward

![graph](../img/RL_graph.JPG)

## Markov Decision Process
> Mathematical formulation of the RL problem
> Markov property : Current state completely characterises the state of the world
> 
![equation](https://latex.codecogs.com/gif.latex?%5C%5C%5Ctextrm%7BDefined%20by%20%3A%20%7D%5C%2C%28%5Cmathcal%7BS%7D%2C%20%5Cmathcal%7BA%7D%2C%20%5Cmathcal%7BR%7D%2C%20%5Cmathbb%7BP%7D%2C%20%5Cgamma%29%5C%5C%20%5Cmathcal%7BS%7D%20%3A%20%5Ctextrm%7Bsef%20of%20possible%20states%7D%20%5C%5C%20%5Cmathcal%7BA%7D%20%3A%20%5Ctextrm%7Bsef%20of%20possible%20actions%7D%20%5C%5C%20%5Cmathcal%7BR%7D%20%3A%20%5Ctextrm%7Bdistribution%20of%20reward%20given%20%28state%2C%20action%29%20pair%7D%20%5C%5C%20%5Cmathbb%7BP%7D%20%3A%20%5Ctextrm%7Btransition%20probability%20i.e.%20distribution%20over%20next%20state%20given%20%28state%2C%20action%29%20pair%7D%20%5C%5C%20%5Cgamma%20%3A%20%5Ctextrm%7Bdiscount%20factor%7D)

<!--stackedit_data:
eyJoaXN0b3J5IjpbMTE0NTM0NDk2NiwtMTgxMTA4MjIxNywyMz
M4NzI4MTBdfQ==
-->