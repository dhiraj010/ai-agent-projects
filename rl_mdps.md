# RL Theory: Markov Decision Processes, Q-Learning, and Value Functions
Notes on MDPs, Q-learning, and value functions from Sutton & Barto’s RL book (Chapter 3) to understand RL’s mathematical foundations.

## Notes from Sutton & Barto Chapter 3
Key points from skimming Chapter 3 of *Reinforcement Learning: An Introduction*:

- **MDP**: A framework for RL, like a game with states (situations), actions, and rewards.
  - Example: My thermostat’s states are temperatures, actions are heating/cooling, rewards are comfort or energy savings.
- **Value Functions**: Numbers showing how good a state or action is.
  - **State-Value (v(s))**: Value of being in a state (e.g., 18°C is bad, -5).
  - **Action-Value (q(s,a))**: Value of an action in a state (e.g., heating at 18°C is good, +10).
- **Q-Learning**: A way to learn the best actions by trying them and updating their value (q(s,a)).
- **Why It’s Useful**: MDPs model problems like my thermostat, value functions guide decisions, and Q-learning helps it learn without fixed rules.

## MDPs, Q-Learning, and Value Functions
A simple explanation of these RL concepts:

- **Markov Decision Process (MDP)**:
  - A framework for decisions, like a map of states, actions, and rewards.
  - **Parts**:
    - **States**: Situations (e.g., thermostat at 18°C).
    - **Actions**: Choices (e.g., heat or cool).
    - **Rewards**: Points (e.g., +10 for comfort).
    - **Transition Probabilities**: How actions change states (e.g., heating raises temperature).
    - **Discount Factor**: Balances now vs. later rewards.
  - Example: My thermostat’s MDP models temperatures, heating/cooling, and comfort.
- **Value Functions**:
  - Numbers showing how good states or actions are.
  - **State-Value (v(s))**: Value of a state (e.g., 22°C is +10).
  - **Action-Value (q(s,a))**: Value of an action (e.g., heating at 18°C is +10).
  - Example: Thermostat learns 22°C is good, heating at 18°C is valuable.
- **Q-Learning**:
  - A method to learn the best actions by trying them and updating q-values.
  - Example: Thermostat tries heating at 18°C, gets a reward, and updates q-value to favor heating.
- **Why It Matters**: MDPs structure my thermostat’s decisions, value functions guide it, and Q-learning lets it learn without fixed rules, unlike my Day 1 agent.