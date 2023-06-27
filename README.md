# NavigationProject_Udacity
This repository contains the files for the navigation project as part of Udacity Nano-Degree Learning program.

![42135619-d90f2f28-7d12-11e8-8823-82b970a54d7e](https://github.com/SAMNaqvi1212/NavigationProject_Udacity/assets/76792427/570bbb97-f4b5-47cf-94b1-a821b00b89e9)
### Introduction Project Navigation
For this project, an agent would be trained to navigate and collect bananas. 

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
 ### Improvements in the model
 Two proposed improvements in the model that we had incorporated are as follows:
 1) Experience Replay
 2) Fixed Q-Targets

### Proposed Modifications:
1) Try to implement Prioritized Experience Replay or Duel DQN (even Rainbow DQN).
2) Create a general DQN architecture that could be used for other architectures.

