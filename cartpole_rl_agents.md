# CartPole RL Agent Documentation
A guide to my CartPole DQN agent, explaining what it does, how it works, and how it connects to my thermostat project.

## What Is It?
My agent is a smart bot that learns to balance a pole on a moving cart in the CartPole game (from Gym). It uses a neural network (called DQN) to decide whether to move the cart left or right to keep the pole upright.

## How It Works
- **Game Setup**: The cart moves on a track, and the pole can fall if not balanced. The bot gets a point for each moment the pole stays up (up to 500).
- **Learning Method**: The bot uses a Deep Q-Network (DQN), a neural network that learns by trying actions and checking rewards. It’s like teaching a kid to ride a bike by trial and error.
- **Training Process**:
  - Starts with random moves, then learns smarter choices.
  - Uses PyTorch to build the neural network (like in `ai_libraries.ipynb`).
  - Saves past moves to learn from them (called experience replay).
- **Key Steps**:
  - Built the agent (`dqn_cartpole_agent.ipynb`).
  - Debugged it (`dqn_cartpole_debug.ipynb`).
  - Tuned settings like learning speed (`hyperparameter_tuning.ipynb`).
  - Tested a pro library, Stable-Baselines3 (`rl_libraries.ipynb`).

## Results
- **Initial Performance**: Random moves scored ~10–30 points.
- **After Training**: My custom DQN hit ~150–200 points after 150 episodes.
- **Tuned Settings**: Faster learning (0.001) gave high scores but was shaky; slower decay (0.999) was smoother.
- **Stable-Baselines3**: Got ~150 points in ~3 min, super easy to use.
- **Plots**: Reward graphs showed scores climbing, proving the bot learned.

## Connection to Thermostat
- My thermostat project (day1_summary.md) needs a bot to adjust temperatures based on sensor data, like the CartPole bot balances the pole.
- The DQN can learn to pick the best temperature settings by trying and checking results, just like moving the cart.
- Stable-Baselines3 could make this faster for my thermostat.

## What I Learned
- **Building RL**: Coding a DQN from scratch is fun but takes time.
- **Debugging**: Checking rewards and errors helped fix issues.
- **Tuning**: Small setting changes (like learning speed) make a big difference.
- **Libraries**: Stable-Baselines3 is awesome for quick projects; Ray RLlib is for bigger ones.
- **Documentation**: Writing this makes my work clear to others (and future me!).

## Next Steps
- Add a “target network” to make the DQN more stable (dqn_intro.md).
- Build a thermostat game setup (Gym environment).
- Try Stable-Baselines3’s PPO algorithm for my thermostat.