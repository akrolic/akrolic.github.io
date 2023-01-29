---
title: "Reinforcement Learning Class Project: Learning Gait Trajectories for a Quadrupedal Robot"
excerpt: "<br/><img src='/images/sim2real.png'>"
collection: portfolio
---

------

This work was completed in Spring 2021 by [Alexander Krolicki](https://www.linkedin.com/in/agkrolicki/) and [Sarang Sutavani](https://www.linkedin.com/in/ssarang/) in ME8930 Reinforcement Learning, taught by [Dr. Umesh Vaidya](https://www.clemson.edu/cecas/departments/me/people/faculty/Vaidya.html). 

[Final Project Report](/files/RL_Project__ME_8930_Krolicki_Sutavani.pdf) | [Final Project Presentation](/files/ME8930 TRPO PPO Final Presentation.pdf) | [TRPO Training Video](https://youtu.be/Z4BZgIL5d0Y) | [Code](https://colab.research.google.com/drive/14gOUZhOGHNf3ZvtpfUbgGGii3tcnbgbv?usp=sharing)

Abstract:

The focus of this paper is to provide insight regarding the importance of policy gradient methods when
applied to continuous systems. We study the development of policy gradient algorithms, and explain
when and how policy gradients should be applied or when they are inadequate for the given problem.
We specifically investigate 2 well known algorithms which utilize policy gradient methods, Proximal
Policy Optimization (PPO) and Trust Region Policy Optimization (TRPO). To better demonstrate
in practice how these algorithms would need to be implemented, we choose to utilize a simulation
environment to train a quadrupedal robot to learn a gait planning and control policy. We demonstrate
the use of developmental tools which help to expedite training, hyper-parameter tuning, and model
analysis. Altogether we present a comparison of these results, and provide qualitative commentary on
the behaviors learned by the quadrupedal robot over time between the two algorithms.

<p align="center">
<img src='/images/sim2real.png'>
<br>
Figure 1. “Minitaur Robot” Transfer of control policy from simulation to physical robot [1].
</p>

References:

[1] Jie Tan, Tingnan Zhang, Erwin Coumans, Atil Iscen, Yunfei Bai, Danijar Hafner, Steven Bohez, and Vincent Vanhoucke. Sim-to-real: Learning agile locomotion for quadruped robots. arXiv preprint arXiv:1804.10332, 2018. 