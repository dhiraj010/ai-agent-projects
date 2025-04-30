# Deep Q-Networks (DQN) Introduction
Notes on deep Q-networks from a YouTube video and simple explanations to understand neural networks in RL.

## Notes from YouTube Video
Key points from a Deep Q-Learning video (e.g., by Siraj Raval):

- DQNs combine Q-learning with neural networks to handle complex environments like games.
- Instead of a Q-table, a neural network predicts Q-values for actions based on the state.
- Example: In an Atari game, the network takes game pixels and outputs move values.
- Experience Replay: Saves past moves to train the network, like reviewing game footage.
- Target Network: A second network stabilizes learning by setting consistent goals.