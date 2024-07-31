# TD Control (On policy and off policy)

In this section we take 5 x 5 grid world with specific characteristics to compare Sarsa and Q-learning algorithms to learn the optimal policy for the environment. Property of grid world environment as below. Agent in environment can take a step up, down, left or right actions. However, If the agent attempts to step off the grid, the location of the agent remains unchanged with reward of −1.
The blue state represents the start point of the episode in given instance. The black state represents terminal state, where reaching either state will terminate that specific episode. The red squares act as a wall where an agent steps on to red state will incur -20 reward and move to blue state. Taking any action in normal states yield -1 reward.

![image](https://github.com/user-attachments/assets/0e0eba91-8eef-42a6-ba93-60c6ea7445e7)

Here we have calculated the optimal policy from below algorithms

  1.	SARSA on policy TD control
  2.	Q-learning (off-policy TD control)

Results can be recreated by running A3Q1.ipynb file

Policy obtained from both algorithms

![image](https://github.com/user-attachments/assets/69de76bb-800d-48bc-8d4b-fc68a247b008)

# Stochastic-gradient and Semi-gradient Methods

In this section we try to evaluate value function of each state by random walk in the 7x7 grid world as in below figure. The characteristics of the grid world can be summarized as below. Each time agent start the episode in the center of the grid world which is highlighted in blue color. Agent is equally likely to move up, down, left, or right at any state. Transition between two states doesn’t incur any reward and trying to step out of grid world leads agent to stay in the same state without any reward as well. Episodes terminate when agent reach any of black highlighted states. However, reaching to top right (0,6) terminal state incur +1 reward and reaching to bottom left corner (6,0) will lead to -1 reward.

![image](https://github.com/user-attachments/assets/815dc91e-fd74-4089-9d0a-20fcca60c950)

Here we have calculated value function from

  1. Exact value function from iterative policy evaluation
  2. Gradient Monte Carlo method
  3. Semi-gradient TD(0) method

Results can be recreated by running A3Q2.ipynb file
  
