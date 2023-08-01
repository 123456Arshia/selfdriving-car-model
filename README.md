# selfdriving-car-model
self driving car using dqn
Self-Driving Car Simulation with Deep Q-Learning (DQN)
his repository contains a Python script that demonstrates a self-driving car simulation using Deep Q-Learning (DQN). The car learns to navigate a 2D grid environment, avoiding obstacles (sand areas), and reaching a specified goal location. The simulation is built using the Kivy framework for GUI and visualization.

Getting Started

To run the self-driving car simulation on your local machine, follow these steps:

Install the required dependencies:
Kivy: pip install kivy
NumPy: pip install numpy
Matplotlib: pip install matplotlib
PyTorch: Refer to the official PyTorch website for installation instructions.
Clone the repository to your local machine.
Run the main.py script to launch the simulation.
Simulation Controls

Drawing Obstacles: The simulation allows the user to draw sand areas (obstacles) on the screen using the left mouse button. The car learns to avoid these areas.
Clearing Obstacles: Click the "Clear" button to remove the drawn sand areas from the screen.
Saving the Learned Model: Click the "Save" button to save the learned model (brain) of the DQN agent. The model will be saved as "last_brain.pth".
Loading a Saved Model: Click the "Load" button to load a previously saved brain for the DQN agent.
How it Works

The simulation uses a Deep Neural Network (DNN) to implement the Q-Learning algorithm with experience replay (DQN).
The car has three sensors that detect obstacles in its vicinity.
The user can draw sand areas on the screen, which the car learns to avoid during training.
The DQN agent is trained through reinforcement learning to maximize its cumulative reward while reaching the goal without entering the sand areas.
The agent learns to adjust its actions (steering) based on the observed states (sensor signals) to navigate the environment effectively.
Notes

This simulation is intended for educational purposes and is a simplified representation of a self-driving car scenario. Real-world self-driving car systems are much more complex and involve safety-critical components.
Training a DQN agent in the Kivy application might require some time, and the performance may vary depending on your hardware.
Author

This project was developed by Arshia as a demonstration of Deep Q-Learning for self-driving car simulations.

Acknowledgments

Special thanks to kiril for providing the base code for the DQN agent and Kivy visualization.
