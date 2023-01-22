# Iterative reward shaping for non-overshooting altitude control of a wing-in-ground craft based on deep reinforcement learning (DRL)
* **Description on directories:**  The codes are presented in seperate dierectory according to the section of 'Cases and analysis' in the manuscript. As for each sub case, eight different seeds are used and the one rewarded mostly is picked as the result. So, there are 8 dierectories at each sub-sub directory.
* **Main code file:** At the each sub-sub directory, there are six files for the training, which are as following:
1. *RL_3to6.py*. It's main function and the training environment and reward function are defined.

2. *run.py*. It's algorithm of training.

3. *replay.py*. It's classes of replay buffer during training.

4. *net.py*. It's classes of neural network for the algorithm of Proximal Policy Optimization (PPO).

5. *agent.py*. It's classes of agents for PPO.

6. *aeropy_fix.py*. It's functions for aerodynamics and kinectics of the wing-in-ground craft during training.

* **Prerequisites for running codes:**  In order to run the code at each sub-sub directory, the file 'datacollection.npy' should be downloaded and then placed in the root directory, meaning that it is placed with 'Case1_Scheme_1_twoitems', etc. Since the website of Github limits the size of files, the necessary file and main results are placed in the same directory and they are upload in onedrive. The link is https://maildluteducn-my.sharepoint.com/:f:/g/personal/huhuan2019_mail_dlut_edu_cn/EnfjpZlH5URIteBXVf55bIUBFbkowtktd30EE767rn5naA?e=R5faeH

* **Main results after running codes:** At the each sub-sub directory of 'Results' (in the onedrive or be downloaded), there are eight files which are the outputs after the training, which are as following:

1. *actor_0.3to0.6_case1_0bu.pth*. It's neural network of the Actor in deep reinforcement learning.

2. *critic_0.3to0.6_case1_0bu.pth*. It's neural network of the Critic in deep reinforcement learning.

3. *critic_target_0.3to0.6_case1_0bu.pth*. It's neural network of the Target of Actor in deep reinforcement learning.

4. *guiyi_0.3to0.6_case1_0bu.pth.npy*. It's memory buffer which is used for normalization during training.

5. *ipython.html*. It's the record of output data by ipython consolo.

6. *plot_learning_curve.jpg*. It's reward curve during training.

7. *quan_recorder.npy*. It's the record of reward for each epoch during training.

8. *The trained trajetory.npy*. It's the trajectory which is rewarded mostly after training.
