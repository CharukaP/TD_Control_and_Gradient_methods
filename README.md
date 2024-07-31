# TD Control (On policy and off policy)

Part 1

In this section we take 5 x 5 grid world with specific characteristics to compare Sarsa and Q-learning algorithms to learn the optimal policy for the environment. Property of grid world environment as below. Agent in environment can take a step up, down, left or right actions. However, If the agent attempts to step off the grid, the location of the agent remains unchanged with reward of −1.
The blue state represents the start point of the episode in given instance. The black state represents terminal state, where reaching either state will terminate that specific episode. The red squares act as a wall where an agent steps on to red state will incur -20 reward and move to blue state. Taking any action in normal states yield -1 reward.

![image](https://github.com/user-attachments/assets/0e0eba91-8eef-42a6-ba93-60c6ea7445e7)

Here we have calculated the optimal policy from below algorithms

