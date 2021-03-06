[//]: # (Image References)

[image1]: https://user-images.githubusercontent.com/10624937/42135619-d90f2f28-7d12-11e8-8823-82b970a54d7e.gif "Trained Agent"

# DQN for Navigation UnityML

This is an implementation of Deep Q Networks (Mnih et al, 2015) for the banana navigation environment in UnityML.

![Trained Agent][image1]

### Project Details
#### Environment
A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana.  Thus, the goal of the agent is to collect as many yellow bananas as possible while avoiding blue bananas.  

The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around agent's forward direction.  Given this information, the agent has to learn how to best select actions.  Four discrete actions are available, corresponding to:
- **`0`** - move forward.
- **`1`** - move backward.
- **`2`** - turn left.
- **`3`** - turn right.

#### Solving the environment

The task is episodic, and in order to solve the environment, the agent must get an average score of +13 over 100 consecutive episodes.

### Getting Started

1. Download the environment from one of the links below.
    - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux.zip) <br>
    - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana.app.zip) <br>
    - Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86.zip) <br>
    - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86_64.zip) <br>

2. See file `requirements.txt` for python dependencies. 

### Instructions
Run file `Navigation.ipynb` to run the agent.  

### Files
* `Navigation.ipynb` - load the environment explore the environment, train the agent or run the trained agent
* `agent.py` contains the agent class 
* `model.py` contains the neural network models the agents employ. 
* `checkpoint.pth` contains trained model weights <br>
* `REPORT.md` contains description of implementation, results, and ideas for future work.<br>

### Reference
* "Human-level control through deep reinforcement learning", Mnih et al, 2015<br>
https://storage.googleapis.com/deepmind-media/dqn/DQNNaturePaper.pdf <br>
