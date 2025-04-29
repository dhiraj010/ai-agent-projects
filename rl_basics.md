# RL Basics: Agent, Environment, Reward, Policy
Notes on reinforcement learning concepts and Lecture 1 of David Silver’s RL Course to understand the RL framework.

## Notes from David Silver’s Lecture 1
Key points from the first 20–30 minutes of the RL Course (Lecture 1):

- RL is about learning by doing, like a kid learning to walk by trying and falling.
- Unlike supervised learning (e.g., my PyTorch example), RL uses rewards, not correct answers.
- **Agent**: The decision-maker (e.g., a game AI).
- **Environment**: The world it acts in (e.g., a game board).
- **Reward**: Points for good actions (e.g., +1 for winning).
- **Policy**: The strategy it learns (e.g., best moves to win).
- Example: An AI playing Atari learns by earning points for high scores.
- Markov Decision Process (MDP): A way to structure RL problems with states, actions, and rewards.

## RL Concepts: Agent, Environment, Reward, Policy
A simple explanation of the core RL concepts:

- **Agent**: The learner who decides what to do, like a player in a game.
  - Example: My thermostat agent could learn to set temperatures.
- **Environment**: The world the agent interacts with, like a house’s temperature system.
  - Example: Includes the room’s temperature and weather.
- **Reward**: Points for good actions, like a game score.
  - Example: +10 for a comfortable room, -5 for wasting energy.
- **Policy**: The strategy the agent learns, like a plan of the best actions.
  - Example: “Heat the room if it’s too cold” (learned, not fixed).
- **How It Works**: The agent acts, the environment responds with a reward, and the agent improves its policy to get more rewards.
- **Why It Matters**: These concepts let me build smarter agents, like a thermostat that learns to save energy, unlike my rule-based one.