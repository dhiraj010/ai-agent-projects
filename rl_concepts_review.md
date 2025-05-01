# RL Concepts Review
A summary of RL theory and a self-quiz to solidify my knowledge from CartPole and other projects.

## RL Theory Summary
Reinforcement Learning (RL) is about teaching a bot to make smart choices by trying actions and earning rewards, like training a pet with treats. Here’s the breakdown:
- **Agent**: The bot, like my CartPole DQN, making decisions.
- **Environment**: The game world, like CartPole’s track and pole.
- **State**: Current game situation, like pole angle and cart position.
- **Action**: What the bot does, like moving left or right.
- **Reward**: Points for good moves, like +1 for keeping the pole up.
- **Policy**: The bot’s plan for picking actions, like choosing the best Q-value.
- **Value Function**: Guesses future rewards for a state, like Q-values in DQN.
- **Q-Function**: Maps actions and states to expected rewards, learned by the DQN.
- **Epsilon-Greedy**: Balances random tries vs. smart choices, like in my tuning (hyperparameter_tuning.ipynb).
- **Markov Decision Process (MDP)**: The math setup of states, actions, and rewards, like a game map.
- **Q-Learning**: Learning the best actions through a table or neural network (DQN).
- **Discount Factor**: Weights future vs. immediate rewards, like gamma=0.99.

## Quiz Results
I quizzed myself on 10 RL terms to check my understanding. Here’s how I did:
- **Agent**: Got it! It’s the bot, like my DQN in dqn_cartpole_agent.ipynb.
- **Environment**: Easy, it’s CartPole’s game world (Gym’s env).
- **State**: Nailed it—pole angle, cart position, etc.
- **Action**: Simple, left or right moves in CartPole.
- **Reward**: Clear, +1 for each step the pole stays up.
- **Policy**: Got it, the strategy for picking actions (DQN’s neural network).
- **Value Function**: Solid, it guesses future rewards (Q-values).
- **Q-Function**: Good, maps state-action pairs to rewards.
- **Epsilon-Greedy**: Knew it from tuning—random vs. smart actions.
- **Discount Factor**: Understood, like gamma=0.99 for long-term rewards.
- **Note**: All correct, but I’ll revisit value function vs. Q-function to stay sharp.

## Connection to Projects
- **CartPole**: My DQN (dqn_cartpole_debug.ipynb) uses a policy to pick actions, Q-function to learn, and epsilon-greedy for exploration.
- **Thermostat**: My project (day1_summary.md) can use a DQN to adjust temps, with states (sensor data), actions (temp settings), and rewards (comfort/energy).
- **Libraries**: Stable-Baselines3 (rl_libraries.ipynb) simplifies RL but uses the same concepts (policy, Q-function).

## Next Steps
- Review value function math in dqn_intro.md.
- Apply RL to a thermostat Gym environment.
- Try Stable-Baselines3’s PPO to see how policies differ.

- Agent: What’s the “player” in RL, like in CartPole?
- Environment: What’s the “game world” the agent interacts with?
- State: What describes the current situation in CartPole?
- Action: What can the CartPole agent do?
- Reward: What does the agent get for keeping the pole up?
- Policy: What’s the agent’s strategy for picking actions?
- Value Function: What does this guess about future rewards?
- Q-Function: What does this tell the agent in Q-learning?
- Epsilon-Greedy: How does this balance random vs. smart actions?
- Discount Factor: How does this affect long-term vs. short-term rewards?