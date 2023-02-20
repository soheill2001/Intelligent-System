# Connect 4 Game with Deep Q-Learning
## Introduction
In this project, we have implemented a deep Q-learning agent for the Connect Four game. Connect Four is a two-player game in which the players take turns dropping discs into a 6x7 grid. The first player to get four discs in a row, column, or diagonal wins the game.

The goal of our agent is to learn how to play the game by interacting with the environment and maximizing the reward it receives. We have used a deep Q-learning algorithm to train the agent, which learns a policy that maps game states to actions.

We have used the Kaggle environment for the Connect Four game, which provides a Python API to interact with the game. We have implemented our agent using TensorFlow and the Keras API.
## Installation
To run this project, you need to install the following packages:

+ `kaggle-environments>=0.1.6`
+ `tensorflow>=2.0.0`

## Running the Code
The main code for our agent is provided in the file connect4.py. To train the agent, you can run the following command:
`python connect4.py`

This will train the agent for 1000 episodes against a random agent. You can modify the number of episodes and the opponent agent in the code.

During the training, the agent will interact with the environment and update its Q-values using the deep Q-learning algorithm. The agent will also gradually reduce its exploration rate, which determines the probability of taking a random action instead of the one recommended by its policy.

After the training, the agent's performance can be evaluated by running the Connect4.run() method with the agent as input. This will play a game between the agent and a random opponent and display the game board in an IPython notebook.

## Architecture
Our agent is implemented using a deep neural network with the following architecture:

+ Input layer: Takes the game state as input, which is a 6x7 matrix of integers representing the current state of the game board.
+ Convolutional layer: Applies a 3x3 convolutional filter with 64 output channels and a ReLU activation function.
+ Convolutional layer: Applies another 3x3 convolutional filter with 64 output channels and a ReLU activation function.
+ Flatten layer: Flattens the output of the convolutional layers into a 1D vector.
+ Dense layer: Applies a fully connected layer with 64 units and a ReLU activation function.
+ Dense layer: Applies another fully connected layer with 128 units and a ReLU activation function.
+ Dense layer: Applies another fully connected layer with 64 units and a ReLU activation function.
+ Output layer: Applies a fully connected layer with 7 units (one for each possible action) and a linear activation function.
The agent uses the following hyperparameters:

+ Epsilon: The exploration rate, which determines the probability of taking a random action instead of the one recommended by the policy. The epsilon value starts at 1 and decays by a factor of 0.995 after each episode.
+ Learning rate: The learning rate of the optimizer, which is set to 0.0001.
+ Loss function: The agent uses the sparse categorical cross-entropy loss function, which is optimized using the Adam optimizer.


## Evaluation
We evaluated our agent by playing it against a random agent and measuring its win rate over multiple games. We found that the agent's win rate increased over time as it learned to make better moves.

We also monitored the agent's average reward per episode during training and found that it