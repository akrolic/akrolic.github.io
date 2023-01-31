---
title: "DIRA - Quadrupedal Robots"
excerpt: "<br/><img src='/images/Quadrupeds.png'>"
collection: portfolio
---

The primary motivation for building quadruped robots in the Distributed Intelligence and Robot Autonomy Lab (DIRA) was to construct a sufficiently complex non-linear dynamical system. The quadruped robots we built in our lab came in several different sizes, each with their own unique leg configurations. I started the lab in 2020 with Dr. Umesh Vaidya and Dr. Yiqiang Han, with basically no initial funding. We had a few thousand dollars to start with, coming mostly from our own pockets. This robotic platform marked the next step in my journey from working on and building drones and ground vehicles in my undergraduate research. 

We decided to start with an open source project, which was affordable and was capable of performing more complex gaits than just the standard trotting or walking gait most off-the-shelf robots are capable of. We decided to build the [Stanford Doggo](https://github.com/Nate711/StanfordDoggoProject), a low-cost, high-powered quadruped robot designed by [Nathan Kau](https://nathankau.com/) and the [Stanford Robotics Club](https://stanfordstudentrobotics.org/doggo). The unique thing about this robot was that it could jump, and at the time held the record for vertical jumping agility, a measure of average vertical speed [1]. 

I can honestly say that this robot taught me so much and I am so grateful to have had the opportunity to learn from the project. All of the students in the DIRA lab that worked on this robot grew their understanding of mechanical, electrical, and computer science applied to robotic systems. The primary focus of my graduate research however, was not to build or design robots, but to bring new theory into practice. 

<p align="center">
<img src='/images/built_not_bought.jpg'>
<br>
Figure 1. Various stages of construction of the Clemson Tigger. 
</p>

We used the robot we built in our lab to conduct experiments to validate the use of operator theory in modeling nonlinear dynamics. In particular, we published a paper to the 2022 Modeling, Estimation, and Controls Conference using this robot, proposing a strictly proprioceptive way of identifying terrain dynamics using the spectral decomposition of the Koopman Generator [2]. 

<p align="center">
<img src='/images/mecc2022.jpg'>
<br>
Figure 2. Presenting at the 2022 Modeling, Estimation, and Controls Conference. 
</p>

<p align="center">
<img src='/images/terrains.png'>
<br>
Figure 3. The soil test bed with several terrain types. 
</p>

We incorporated the Robotics Operating System (ROS) into the system to be able to collect time-synchronized snapshots of the leg positions, setpoints, and motor currents. This required constructing custom ROS messages so as to package all the information into one topic, so that the microcontroller would be able to transmit the information at a high frequency. Using these measured values, we derived quantities such as the motor torques, foot forces, and the cartesian position of the foot. This made conducting multiple experiments and collecting data stright forward using rosbag's and rqt. 

<p align="center">
<img src='/images/ros_tigger.png'>
<br>
Figure 4. Integrating ROS into Clemson Tigger for data collection. 
</p>

I spent most of my time researching new techniques for solving the nonlinear optimal control problem, since this is a fundamentally difficult problem, particularly for quadruped robots since they can be modeled as switched systems. I explored reinforcement learning based methods for obtaining policies for learned gaits, but it was quickly evident that there was no way to produce formal guarantees on stability of the learned policies, and performing the sim2real transformation was itself a uncertain task. Thankfully we have made major breakthroughs in solving the optimal control problem, and PhD student [Sriram S.K.S Narayanan](https://www.linkedin.com/in/sriramsundarks/) and MSME [Andrew Zhang](https://www.linkedin.com/in/andrewzheng11/) have been working towards researching novel control algorithms based on our new developments in optimal control theory. 

In the meantime, there have been plenty of suboptimal solutions using MPC, and other more complex deep reinforcement learning methods coming out of MIT, USC, and ETH Zurich to name a few. The machinery and expertise employed by these groups trumps our, but we are proud of what we have been able to accomplish learning from this project and others publications in the past two years. 

In order to make the control problem simpler, it is desirable to reduce the number of degrees of freedom of the robot, but still be able to retain the manuverability of the legs. In Fall 2022, [Jackson Erb]() joined our lab and conducted his undergraduate honors thesis research on the design and integration of a wheel-leg actuator for our Clemson Tigger Robot. I mentored Jackson throughout the entire process and in the end we came up with a design which was able to be integrated into the existing coaxial output shafts.

<p align="center">
<img src='/images/wheel-leg.png'>
<br>
Figure 5. Clemson Tigger wheel-leg design and fabrication. 
</p>

We will soon be validating the performance of this new wheel-legged system this semester, and we will open-source this project for others interested in implenting this type of actuator on their own robot.

During the Summer of 2022, I challanged [Jackson Erb](https://www.linkedin.com/in/jackson-erb-327b01207) and [Graham Lancaster](https://www.linkedin.com/in/grlanca) to come up with a scaled up version of Clemson Tigger which was capable of carrying additional onboard sensors and an embedded compute platform so that we could further research autonomous off-road control and navigation algorithms. With the generous support of Dr. Umesh Vaidya, we completed a design which incorporated a passive suspension system which could be dynamically engaged and disengaged so that the motors were not always doing all the heavy lifting. This would enable the system to reject high frequency disturbances at speed, but still provide the flexibility of moving the arms above large obstacles with the suspension disengaged. 

<p align="center">
<img src='/images/TiggerXL.png'>
<br>
Figure 6. Clemson Tigger XL Concept Design. 
</p>

This is a complex design concept, completed in a short amount of time. Depending on future funding, this project may be built and iterated on by future students of the DIRA lab. 



References:

[1] N. Kau, A. Schultz, N. Ferrante and P. Slade, "Stanford Doggo: An Open-Source, Quasi-Direct-Drive Quadruped," 2019 International Conference on Robotics and Automation (ICRA), Montreal, QC, Canada, 2019, pp. 6309-6315, doi: 10.1109/ICRA.2019.8794436.

[2] A. Krolicki, D. Rufino, A. Zheng, S. Narayanan, J. Erb, U. Vaidya, "Modeling Quadruped Leg Dynamics on Deformable Terrains using Data-driven Koopman Operators." IFAC-PapersOnLine, Volume 55, Issue 37, 2022, Pages 420-425, ISSN 2405-8963, doi: 10.1016/j.ifacol.2022.11.219.