Snakey-Boi: Reinforcement Learning-Based Snake Game AI
=======================================================

Project Overview:
-----------------
This project implements a self-learning agent that plays the classic Snake game using Deep Q-Learning. 
The environment is built using Pygame, and the learning model is implemented with PyTorch.

The goal is to provide a hands-on demonstration of reinforcement learning principles such as state representation, 
reward optimization, and experience replay.

Repository Structure:
---------------------
- agent.py         : Core training loop and reinforcement learning logic
- game.py          : Snake game environment implemented using Pygame
- helper.py        : Neural network model (Q-network) and training utilities
- plot_helper.py   : Real-time training visualization using Matplotlib
- requirements.txt : List of project dependencies
- model/           : Directory for saving trained model checkpoints (e.g., model.pth)

Setup Instructions:
-------------------
1. (Recommended) Create and activate a virtual environment:

   Linux/macOS:
   $ python3 -m venv venv
   $ source venv/bin/activate

   Windows:
   > python -m venv venv
   > venv\Scripts\activate

2. Upgrade pip (recommended):
   $ python -m pip install --upgrade pip

3. Install the required dependencies:
   $ pip install -r requirements.txt

4. Start training the AI agent:
   $ python agent.py

   A game window will appear, and a live plot of training scores will be displayed.
   The agent will gradually improve its performance through trial and error.

Model Saving:
-------------
Model checkpoints are saved in the `model/` directory when the agent achieves a new high score.

Key Concepts Demonstrated:
--------------------------
- Deep Q-Learning with epsilon-greedy strategy
- Experience replay buffer (short-term and long-term memory)
- State-based decision making
- Reward-driven learning
- Live training performance visualization

Dependencies:
-------------
- torch >= 2.0.0
- pygame >= 2.1.0
- numpy >= 1.23.0
- matplotlib >= 3.5.0
- ipython >= 8.0.0

Future Enhancements:
--------------------
- Implement evaluation mode to run a trained agent without further learning
- Improve state representation (e.g., image-based inputs using CNNs)
- Add a graphical dashboard for performance monitoring
- Extend to support multiple agents or competitive training

Author:
-------
Developed by Shibezz  
GitHub: https://github.com/Shibezz

This project was created as part of an effort to explore practical applications of reinforcement learning 
within game-based environments.
