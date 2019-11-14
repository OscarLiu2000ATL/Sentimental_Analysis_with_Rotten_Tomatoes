# Sentimental_Analysis_with_Rotten_Tomatoes

<img src="./Train_Test_Data/屏幕快照 2019-03-02 上午2.23.29.png" height="400" />

## Overview


## Installation, Testing, Training:

<img src="./User Guide.pdf" height="400" />

## What is Double Dueling Deep Q-Network?
It is a variant of the Deep Q-learning network. The Double DQN uses two systems, Q and Q'(target network), to determine action and value, respectively. In doing so, it prevents overestimation. 

The Dueling DQN uses two streams after the convolution layers, namely V(s) and A(s, a). Q(s, a) is the aggregation of V(s) and the normalized A(s, a). This change in network structure makes updates of Q values of the state, action pair more efficient (we can only sample so much data). 

## Network Architecture
<img src="./images/drawing.png" width = "1000"  />

#### please imagine the depth :D

## Implementetion Tips

#### The Voting System
Normally the random step is to pick an action at random. However, the bird agent runs in 30 FPS and 1 APF (Action per Frame), which means a 50% chance of flapping results in the bird continuously flying into the ceiling. Here I used a 90% chance for falling and a 10% chance for flapping.

## Further Implementations

* Web UI developement
