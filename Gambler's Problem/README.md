# Gambler's Problem

This is a Python implementation of the Gambler's Problem. The problem involves a gambler who wants to reach a goal of winning a certain amount of money by placing bets on a fair coin. Each bet the gambler places is for a fixed amount of money, and if the coin comes up heads, the gambler wins that amount of money, otherwise they lose that amount. The gambler starts with an initial capital of 0 and can place bets until they either reach their goal or lose all of their money.

## How to Use
The code is written in Python and requires numpy and matplotlib libraries. The implementation of the Gambler's Problem is done using the Value Iteration algorithm.

You can run the code in any Python environment of your choice, such as Jupyter Notebook or Spyder. Simply copy the code and run it in the environment.

To change the probability of winning, change the value of p_h in the code to any number between 0 and 1.

To change the goal amount of the gambler, change the value of states in the code to the desired number.

The code implements the Value Iteration algorithm to find the optimal policy for the Gambler's Problem. The algorithm is applied to find the optimal policy for two different probabilities of winning a coin toss: 0.25 and 0.55. The code also plots the optimal policy and the optimal value function for each probability.

The code outputs two graphs for each probability value - a bar chart of the optimal policy for each state, and a line graph of the optimal value function for each state.