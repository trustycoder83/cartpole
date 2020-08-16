# CartPole-v0
A pole is attached by an un-actuated joint to a cart, which moves along a frictionless track. The system is controlled by applying a force of +1 or -1 to the cart. The pendulum starts upright, and the goal is to prevent it from falling over. A reward of +1 is provided for every timestep that the pole remains upright. The episode ends when the pole is more than 15 degrees from vertical, or the cart moves more than 2.4 units from the center.

## OpenAI Gym
OpenAI Gym is a toolkit for developing and comparing reinforcement learning algorithms. It supports teaching agents everything from walking to playing games like pong or pinball. Gym is an open source interface to reinforcement learning tasks.

## Requirements
- [Python 3.6 or 3.7](https://www.python.org/downloads/release/python-360/)
- [CUDA Toolkit 10.1](https://developer.nvidia.com/cuda-10.1-download-archive-base)
- [cuDNN v7.6.5](https://developer.nvidia.com/cuda-10.1-download-archive-base)
- [Pipenv](https://pypi.org/project/pipenv/)

## How to install the packages
You can install the required Python packages using the following command:
- `pipenv sync`

## Deep Q-learning with Experience Replay
A deep Q network (DQN) (Mnih et al., 2013) is an extension of Q learning, which is a typical deep reinforcement learning method. In DQN, a Q function expresses all action values under all states, and it is approximated using a convolutional neural network. Using the approximated Q function, an optimal policy can be derived. In DQN, a target network, which calculates a target value and is updated by the Q function at regular intervals, is introduced to stabilize the learning process. In DQN, learning is stabilized through a heuristic called experience replay (Lin, 1993) and the use of a target network. Experience replay is a technique that saves time-series data in a buffer called replay memory.

## How to run it
You can run the script using the following command: 
- `pipenv run python dqn_cartpole.py`

## Improvement ideas
- improve the code quality
- remove unnecessary comments
