# Iterative reward shaping for non-overshooting altitude control of a wing-in-ground craft based on deep reinforcement learning
* **Description:**  The codes are presented in seperate dierectory according to the section of 'Cases and analysis' in the manuscript. As for each sub case, eight different seeds are used and the one rewarded mostly is picked as the result. So, there are 8 dierectories at each sub-sub directory.
* **Prerequisites:**  In order to run the code at each sub-sub directory, the file 'datacollection.npy' should be downloaded and then placed in the root directory, meaning that it is placed with 'Case1_Scheme_1_twoitems', etc. Since the website of Github limits the size of files, the necessary file and main results are placed in the same directory and they are upload in onedrive. The link is https://maildluteducn-my.sharepoint.com/:f:/g/personal/huhuan2019_mail_dlut_edu_cn/EnfjpZlH5URIteBXVf55bIUBFbkowtktd30EE767rn5naA?e=R5faeH

* **Results:** At the each sub-sub directory of 'Results' (in the onedrive or be downloaded), there are eight files which are the outputs after the training, which are as following:

1. *actor_0.3to0.6_case1_0bu.pth*. It's neural network of the Actor in deep reinforcement learning (DRL).

2. *critic_0.3to0.6_case1_0bu.pth*. It's neural network of the Critic in deep reinforcement learning (DRL).

3. *critic_target_0.3to0.6_case1_0bu.pth*. It's neural network of the Target of Actor in deep reinforcement learning (DRL).

4. *guiyi_0.3to0.6_case1_0bu.pth.npy*. It's memory buffer which is used for normalization during training.

5. *ipython.html*. It's the record of output data by ipython consolo.

6. *plot_learning_curve.jpg*. It's reward curve during training.

7. *quan_recorder.npy*. It's the record of reward for each epoch during training.

8. *The trained trajetory.npy*. It's the trajectory which is rewarded mostly after training.
