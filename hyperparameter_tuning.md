## Experiment Results
Documenting hyperparameter tuning results for CartPole DQN.

### Setup
- **Baseline**: `learning_rate=0.0005`, `epsilon_decay=0.995`, `gamma=0.99`
- **Fast Learning**: `learning_rate=0.001`, `epsilon_decay=0.999`, `gamma=0.99`
- **Long-Term Focus**: `learning_rate=0.0005`, `epsilon_decay=0.995`, `gamma=0.999`
- Ran 100 episodes each, plotted rewards with matplotlib.

### Results
- **Baseline**: Rewards reached ~150–200 by episode 100, steady learning curve.
- **Fast Learning**: Hit ~100–200 faster but had some dips (unstable at high `learning_rate`).
- **Long-Term Focus**: Slower climb, reached ~120–180, smoother curve (high `gamma`).
- **Plot**: All trended up, Fast Learning peaked highest but was shaky.

### Insights
- **Learning Rate**: Higher `learning_rate` (0.001) speeds learning but risks instability.
- **Epsilon-Greedy**: Slower `epsilon_decay` (0.999) keeps exploration longer, good for complex tasks.
- **Discount Factor**: Higher `gamma` (0.999) focuses on long-term rewards, smoother but slower.
- **For Thermostat**: Use moderate `learning_rate` (0.0005–0.001) and high `gamma` (0.99) for stable learning (`day1_summary.md`).
- **Next**: Try `epsilon_decay=0.997` or add target network (`dqn_intro.md`).