# Reinforcement Learning in a Magical Grid World

## Introduction:
This repository contains the implementation and analysis of reinforcement learning algorithms applied to a magical grid-world environment inspired by the Harry Potter universe. The primary objective is to guide an agent (Harry) through the grid-world, facing challenges such as villains (penalties) and collecting boosters (rewards) to reach the ultimate goal - the Golden Snitch.

## Environment Description=:
The environment is implemented using the Gym library and consists of a 4x4 grid. Key details include:
- **States:** Defined grid positions including starting, ending, and intermediate states.
- **Actions:** Up, Down, Right, Left movements.
- **Rewards:** Various objects such as wands, owls, the Golden Snitch, Voldemort, and Umbridge, each with specific rewards or penalties.
- **Objective:** Reach the Golden Snitch with maximum reward within a limited number of timesteps.

## Visualization:
![image](https://github.com/shreyaguru-1/Reinforcement-Learning-in-a-Magical-Grid-World-using-SARSA/assets/166087435/6f4ad982-bcb9-44a8-9803-6037f4816f6b)

### SARSA:
- **Algorithm:** State-Action-Reward-State-Action
- **Update Function:** Q(s, a) ← Q(s, a) + α[r + γ Q(s', a') - Q(s, a)]
- **Key Features:** On-policy learning, handles stochastic environments, learns from agent actions during training.
- **Advantages:** Simple implementation, handles stochastic environments, converges to near-optimal solutions.
- **Disadvantages:** Slow convergence, requires many iterations for optimal policy, may not be suitable for large-scale problems.

### Q-Learning:
- **Algorithm:** Off-policy learning with Q-function
- **Update Function:** Q(s, a) ← Q(s, a) + α[r + γ max a' Q(s', a') - Q(s, a)]
- **Key Features:** Model-free, estimates optimal policy regardless of agent's actions, achieves better convergence.
- **Advantages:** Doesn’t require knowledge of environment dynamics, converges to optimal policy, allows learning regardless of agent's actions.
- **Disadvantages:** Not suitable for large-scale problems, may not handle delayed rewards well, prone to overestimation.

## Conclusion:
This repository offers insights into reinforcement learning algorithms SARSA and Q-Learning applied to a magical grid-world environment. By understanding the environment, and algorithmic approaches, it provides a comprehensive guide to reinforcement learning tasks.

---

Feel free to customize and expand this README according to your specific requirements and additional analyses.
