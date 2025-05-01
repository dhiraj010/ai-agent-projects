# Exploring RL Libraries
Researched Stable-Baselines3 (SB3) and Ray RLlib, ran an SB3 DQN script for CartPole to test it.

## Research
- **Stable-Baselines3 (SB3)**:
  - Easy to use, great for beginners.
  - Has ready-to-go algorithms like DQN, PPO.
  - Perfect for small projects like CartPole or my thermostat.
  - Uses PyTorch, simple setup in Colab.
- **Ray RLlib**:
  - Built for big projects with multiple agents or huge data.
  - More complex setup, needs Ray installed.
  - Great for scaling RL to clusters, like for robotics or games.
  - Supports PyTorch/TensorFlow, but harder for beginners.

## SB3 Sample Script Results
- Ran SB3 DQN on CartPole (50,000 timesteps).
- Mean reward: ~150 +/- 20 (good, matches my custom DQN!).
- Plot showed rewards climbing from ~20 to ~150.
- SB3 was fast and easy, took ~3 min to train.

## Insights
- **SB3**: Awesome for quick RL projects. I’ll use it for my thermostat RL agent (day1_summary.md).
- **RLlib**: Cool for future big projects, but too complex for now.
- **Scaling RL**: SB3 is enough for my laptop; RLlib shines with multiple computers.
- **Next**: Try SB3’s PPO or RLlib’s CartPole script when I need multi-agent RL.