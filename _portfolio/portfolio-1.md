---
title: "DIRA - Quadrupedal Robots"
excerpt: "<br/><img src='/images/Quadrupeds.png'>"
collection: portfolio
---

The primary motivation for building quadruped robots in the Distributed Intelligence and Robot Autonomy Lab (DIRA) was to construct a sufficiently complex non-linear dynamical system. The quadruped robots we built in our lab came in several different sizes, each with their own unique leg configurations. I started the lab in 2020 with Dr. Umesh Vaidya and Dr. Yiqiang Han, with basically no initial funding. We had a few thousand dollars to start with, coming mostly from our own pockets. This robotic platform marked the next step in my journey from working on and building drones and ground vehicles in my undergraduate research. 

We decided to start with an open source project, which was affordable and was capable of performing more complex gaits than just the standard trotting or walking gait most off-the-shelf robots are capable of. We decided to build the [Stanford Doggo](https://github.com/Nate711/StanfordDoggoProject), a low-cost, high-powered quadruped robot designed by [Nathan Kau](https://nathankau.com/) and the [Stanford Robotics Club](https://stanfordstudentrobotics.org/doggo). The unique thing about this robot was that it could jump, and at the time held the record for vertical jumping agility, a measure of average vertical speed [1]. 

I can honestly say that this robot taught me so much and I am so grateful to have had the opportunity to learn from the project. All of the students in the DIRA lab that worked on this robot grew their understanding of mechanical, electrical, and computer science applied to robotic systems. The focus of my graduate research however was never to build or design robots, but to bring new theory into practice. 

We used the robot we build in our lab to conduct experiments to validate the use of operator theory in modeling nonlinear dynamics. In particular, we published a paper to the 2022 Modeling, Estimation, and Controls Conference using this robot, proposing a strictly proprioceptive way of identifying terrain dynamics using the spectral decomposition of the Koopman Generator [2]. 


<p align="center">
<img src='/images/terrains.png'>
<br>
Figure 1. The soil test bed with several terrain types. 
</p>



References:

[1] N. Kau, A. Schultz, N. Ferrante and P. Slade, "Stanford Doggo: An Open-Source, Quasi-Direct-Drive Quadruped," 2019 International Conference on Robotics and Automation (ICRA), Montreal, QC, Canada, 2019, pp. 6309-6315, doi: 10.1109/ICRA.2019.8794436.

[2] A. Krolicki, D. Rufino, A. Zheng, S. Narayanan, J. Erb, U. Vaidya, "Modeling Quadruped Leg Dynamics on Deformable Terrains using Data-driven Koopman Operators." IFAC-PapersOnLine, Volume 55, Issue 37, 2022, Pages 420-425, ISSN 2405-8963, doi: 10.1016/j.ifacol.2022.11.219.