# NavigationProject_Udacity
This project is the first one in Udacity's Deep Reinforcement Learning Nanodegree. In this project, I have trained an agent to navigate and collect bananas in a large square world.

![42135619-d90f2f28-7d12-11e8-8823-82b970a54d7e](https://github.com/SAMNaqvi1212/NavigationProject_Udacity/assets/76792427/570bbb97-f4b5-47cf-94b1-a821b00b89e9)
### Introduction Project Navigation
A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana. Thus, the goal of your agent is to collect as many yellow bananas as possible while avoiding blue bananas.
The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around agent's forward direction. Given this information, the agent has to learn how to best select actions. 

The agent will have four possible actions and it has to choose one of the possible actions on each timestep. 
1) Move forward
2) Move backward
3) Move Left
4) Move Right

The agent would be deemed successful if it has been able to collect +13.0 rewards over 100 episodes. 
# Getting Started
First step is to download the environment based on the operating system a person has. Following are the operating systems that are
available, 
1) [Linux](https://learn.udacity.com/nanodegrees/nd893/parts/cd0373/lessons/523b5d7a-053e-4627-a4ac-cee97b8a1ad0/concepts/4c1b4caf-2d7e-4d9f-b7e5-4f7b855f7f1e) 

2) [Mac OSX](https://learn.udacity.com/nanodegrees/nd893/parts/cd0373/lessons/523b5d7a-053e-4627-a4ac-cee97b8a1ad0/concepts/4c1b4caf-2d7e-4d9f-b7e5-4f7b855f7f1e)
   
3) [Windows (32-bit)](https://learn.udacity.com/nanodegrees/nd893/parts/cd0373/lessons/523b5d7a-053e-4627-a4ac-cee97b8a1ad0/concepts/4c1b4caf-2d7e-4d9f-b7e5-4f7b855f7f1e)

4) [Windows (64-bit)](https://learn.udacity.com/nanodegrees/nd893/parts/cd0373/lessons/523b5d7a-053e-4627-a4ac-cee97b8a1ad0/concepts/4c1b4caf-2d7e-4d9f-b7e5-4f7b855f7f1e)


After downloading the environment you can setup your environment accordingly. However, one can also work in the workstation provided by Udacity which has pre-installed all of the libraries and
core requirements required of a system. 

### Methodology
In this project, we used a deep neural network in order to train the agent. The deep neural network comprised of three linear units and two rectified linear layers. The first linear layer comprised of 1024 units and the other layer used 256 neurons. 
The Rectified Linear Layer Unit was used as an activation function here. The model used ADAM optimizer to update the weights regularly. 

### More Innovative Ideas

###Double Deep Q-Networks (DDQN):

One issue with Deep Q-Networks is they can overestimate Q-values (see Thrun & Schwartz, 1993). The accuracy of the Q-values depends on which actions have been tried and which states have been explored. If the agent hasn't gathered enough experiences, the Q-function will end up selecting the maximum value from a noisy set of reward estimates. Early in the learning process, this can cause the algorithm to propagate incidentally high rewards that were obtained by chance (exploding Q-values). This could also result in fluctuating Q-values later in the process

We can address this issue using Double Q-Learning, where one set of parameters w is used to select the best action, and another set of parameters w' is used to evaluate that action.

###Prioritized Experience Replay:

Experience replay lets online reinforcement learning agents remember and reuse experiences from the past. In prior work, experience transitions were uniformly sampled from a replay memory. However, this approach simply replays transitions at the same frequency that they were originally experienced, regardless of their significance. To replay important transitions more frequently, and therefore learn more efficiently, we use prioritized Experience Replay

###Dueling Agents:

Dueling networks utilize two streams: one that estimates the state value function V(s), and another that estimates the advantage for each action A(s,a). These two values are then combined to obtain the desired Q-values.

### Proposed Modifications:
1) Try to implement Prioritized Experience Replay or Duel DQN (even Rainbow DQN).
2) Create a general DQN architecture that could be used for other architectures.

