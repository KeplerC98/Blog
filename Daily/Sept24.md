## Reinforcement Learning (Chapter 16)
a software agent makes **observations** and takes **actions** within an **environment**, and in return it receives **rewards**.
It is used to maximize expecteed long-term rewards

#### Applications
* walking robot
* playing game 
* stock price 

Policy: The algorithm used by the software agent to determine its actions
policy search: brute force approach that try out different values for parameters 
genetic algorithm: create 100 policies randomly and kill 80 worst policies and make 20 survivors to produce 4 offsprings each, which just some random variation on original values 


> we are picking a random action based on the probability given by the neural network, rather than just picking the action with the highest score. This approach lets the agent find the right balance between exploring new actions and exploiting the actions that are known to work well

Another guidance is discount rate r for each step. There has to be a good or bad in situations, by credit assignment problem.

#### Policy gradient