Snake Game AI using Deep Q-Learning
-----------------------------------

This project implements an AI agent that learns to play the classic Snake game using Deep Q-Learning (DQN). It is built from scratch using Python, PyTorch, NumPy, and Pygame.

------------------------
Features
------------------------
- Custom Snake game built using Pygame
- Deep Q-Learning agent with:
    • Epsilon-greedy exploration
    • Experience replay buffer
    • Feedforward neural network
- Real-time score plotting with Matplotlib
- Automatic model saving (best performance)
- Clean, modular codebase

------------------------
Concepts Used
------------------------
1. Reinforcement Learning:
    • Q-Learning
    • Bellman Equation
    • Exploration vs. Exploitation (Epsilon-greedy)
    • Experience Replay

2. Deep Learning:
    • Neural Network with PyTorch
    • ReLU activation, Adam optimizer
    • MSE loss function

3. Game AI:
    • Custom grid environment with collisions
    • Game state encoding
    • Reward design

------------------------
Model Architecture
------------------------
A simple two-layer neural network is used to approximate Q-values.

- Input Layer: 11-dimensional game state
- Hidden Layer: 256 neurons (ReLU activation)
- Output Layer: 3 values representing Q-values for actions:
    [0, 1, 0] → turn right
    [1, 0, 0] → move straight
    [0, 0, 1] → turn left

------------------------
Project Structure
------------------------
agent.py       - RL agent and training loop  
game.py        - Snake game logic using Pygame  
model.py       - Neural network and trainer (PyTorch)  
helper.py      - Live plotting utility   
requirements.txt - includes all the needed libraries

------------------------
How to Run
------------------------
1. Install dependencies manually:
    pip install torch pygame numpy matplotlib ipython

2. Start training:
    python agent.py

------------------------
Author
------------------------
Mohit Methi  
