## Implement Actor-Critic with Transfer Learning for Control Problems

### Section 1: Training Individual Networks
- Adapted actor-critic architecture for Acrobot-v1 and MountainCarContinuous-v0, in addition to retraining for CartPole-v1.
- Ensured identical input and output sizes across tasks with padding and "empty" actions.
- Provided statistics on running time and training iterations for each task.

### Section 2: Fine-Tuning Existing Models
- Fine-tuned models from Acrobot to CartPole and CartPole to MountainCar.
- Re-initialized weights of the output layer for transfer.
- Compared statistics on running time and training iterations with Section 1, analyzed convergence speed.

### Section 3: Transfer Learning with Progressive Networks
- Implemented simplified Progressive Networks for {Acrobot, MountainCar} -> CartPole and {CartPole, Acrobot} -> MountainCar.
- Connected fully-trained source networks to untrained target network, kept source networks frozen.
- Connected hidden layers of source networks to output of target network, based on the number of hidden layers.
- Provided statistics on running time and training iterations, evaluated improvement in training due to transfer learning.
