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

## Cart Pole:
<table>
  <tr>
    <td><img src="https://github.com/sagivantebi/Deep_Reinforcement_Learning-Final_Drill/assets/84729141/c7f460aa-8725-4220-b0f0-e7594c443e45" width="300" height="200"></td>
    <td><img src="https://github.com/sagivantebi/Deep_Reinforcement_Learning-Final_Drill/assets/84729141/08f7499e-9ec7-4938-89ea-f5d56d443fd8" width="300" height="200"></td>
  </tr>
</table>



## Acrobot:

 <img src="https://github.com/sagivantebi/Deep_Reinforcement_Learning-Final_Drill/assets/84729141/838b7e64-99be-489c-a35d-e97b411c1c5d" width="300" height="200"><img src="https://github.com/sagivantebi/Deep_Reinforcement_Learning-Final_Drill/assets/84729141/e8aee2a8-3453-4d30-be60-86b5c4b5de6c" width="300" height="200">

## Mountain Car:

<img src="https://github.com/sagivantebi/Deep_Reinforcement_Learning-Final_Drill/assets/84729141/7078e424-3303-4216-86c1-bccd353ac3b1" width="300" height="200">
<img src="https://github.com/sagivantebi/Deep_Reinforcement_Learning-Final_Drill/assets/84729141/a313242c-d063-41a4-9d99-17c904599f6c" width="300" height="200"> 
