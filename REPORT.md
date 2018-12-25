## Project Report
### Learning Algorithm
This project uses Deep Q Learning (Mnih et al, 2015), which combines Q Learning with deep learning. 

Q-learning is a off-policy temporal difference learning algorithm (Watkins,1989). One-step Q Learning is defined by
Q(s_t, a_t) <- Q(s_t, a_t) + α[r_t+1 + γ max_a Q(s', a) - Q(s_t, a_t)]

In Deep Q Learning, both the current Q value and future Q value are approximated using a neural network, where we try to minimize the TD error. 
Δw = α[r_t+1 + γ max_a Q(s', a) - Q(s_t, a_t)] ▼w Q(s, a, w)


#### Model Architecture
The neural network has the following architecture: 
Input layer is equal to the states vector = 37
First hidden layer consists of 128 nodes
Second hidden layer consists of 64 nodes
Output layer is equal to the length of actions vector = 64


#### Hyperparameters
Discount rate (GAMMA) = 0.99
Maxinum steps per episode (max_t) = 1000

Starting epsilon = 1
Ending epsilon = 0.01
Epsilon decay = 0.99

Update rate of target parameter = 1e-3
Frequecy in updating the network = 4

Buffer size = 1e5
Minibatch size = 64
Learning rate = 5e-4


### Plot of Rewards



### Ideas for Future Work
To employ more techniques in Deep Q Learning for better performance. This includes:
1. Prioritized Experience Replay
2. Dueling DQN
3. Double Q Learning
4. Rainbow - combined imporvements techniques in DQN