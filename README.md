# RL_Frozen-Lake
*   Implemented a frozen lake scenario given the inputs, number of holes (M) and size of the lake (N) (Assumed the lake is square). Starting point will be (0, 0) and goal will be to reach at (N-1, N-1)
*   Implemented Q-learning (Reinforcement Learning method) to learn a path from start to goal.
*   Used the following reward scheme: 50 points on reaching the goal, -50 points on stepping on a hole.
*   Plotted the rewards v/s episodes graphs for various values of learning rate and reduction factor of return.

# Basic steps
*   Each time our model chooses whether to explore(take action randomly) or to exploit(take action based on the best Q-value)
*   Then our model calculates the Q values for each state (states are here cells in the lake ) and each action from the cell (Up ,Down ,Right , Left).
*   It uses Bellman Optimality equation which gives the optimal Q values ,using which we can compute the loss and learn from it.
*   The model runs 3000 episodes and finally we get the optimal Q value for each cell in the lake using which we can take the optimal action to reach the goal from the start
