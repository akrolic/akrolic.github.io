---
title: "CAST - Unmanned Aerial Vehicles (UAV)"
excerpt: "<br/><img src='/images/Drones.jpg'>"
collection: portfolio
---

The Clemson Autonomous Systems Team gitbook documentation can be accessed [here](https://clemson-autonomous-systems.gitbook.io/clemson-university-autonomous-systems/development-projects), a summary of my contributions and collaberations are given below. 

When I was a undergraduate student in Spring 2018, [Dr. Yiqiang Han](https://www.clemson.edu/cecas/departments/me/people/faculty/han.html) invited me to join his undergraduate research group who was focused on building, developing, and testing unmanned aerial vehicles. At that time, [Duncan Nicholson](https://www.linkedin.com/in/duncanicholson/) was the team lead, and he taught me all of the fundamentals of ROS, linux, and the hardware associated with the drone. 

<p align="center">
<img src='/images/foci2018.JPG'>
<br>
Figure 1. FoCI 2018 event showcasing the Intel Aero HiL Simulation in Gazebo. 
</p>

Our team began our journey into the autonomous drone world by experimenting with the [Intel Aero](https://docs.px4.io/main/en/complete_vehicles/intel_aero.html), an out of the box solution that allowed our team to hit the ground running on learning new techniques and algorithms on a capable computing platform. We eventually retired the development of the Aero Drone due to its limitations and restrictions in pursuing more open source solutions.

Our first in house drone was designed to compete in the Vertical Flight Societies (VFS) [7th Annual MAV Student Challange](https://vtol.org/education/micro-air-vehicle-student-challenge/micro-air-vehicle-student-challenge-2019). The competition required that we construct a micro autonomous drone(<500g) to navigate and complete an indoor course with a variety of objectives to complete such as picking up a payload and dropping it off at a designated location. These technical challanges, combined with the hardware limitations at the time, made this difficult for us to complete the qualifying requirements in time to attend the event. This was also the first year of our research group's experience in building autonomous systems. It was a great learning exercise and motivation for all of us and in the end we built our first edge autonomous drone using the NVIDIA TX2 stacked on top of a px4 racer flight controller. 

<p align="center">
<img src='/images/muav.png'>
<br>
Figure 2. Micro autonomous drone - designed for the 7th Annual MAV Student Challange. 
</p>

Starting in Fall 2019, I was given the reigns and lead the UAV undergraduate research group. I started working on the [NVIDIA Redtail Project]() and the [Generalized Autonomy Aviation System](https://gaas.gitbook.io/guide/software-realization-build-your-own-autonomous-drone/gaas-zong-lan) (GAAS) Project. Both of these projects represented a progression in the capabilities of our team to build and develop more advanced autonomous systems. 

I built two Redtail drones, one for the university and another for my own personal use. I affectionately named my drone Lt. Dan from the Forest Gump movies, since during early testing, crashing would lead to broken legs. Despite the challanges of testing these systems, we did so safely and in the Summer of 2020 we were able to autonomously navigate for 6 minutes over 300 meters at a remote trail using the TrailNet deep learning algorithm for navigation [2]. 

<p align="center">
<img src='/images/redtail.jpg'>
<br>
Figure 3. NVIDIA Redtail Drones - Summer 2020. 
</p>

<p align="center">
<img src='/images/foci2020.png'>
<br>
Figure 4. We showcased our work at the Summer 2020 FoCI event at Clemson University.
</p>

Beyond just navigation, we experimented with several simultaneous localization and mapping (SLAM) algorithms using visual inertial odometry obtained from the stereo camera. In order to run these CPU intensive algorithms alongside the GPU based DNN navigation algorithm, I had to modify the drone to accomodate for the heatsync and fans. 

<p align="center">
<img src='/images/hotdrone.png'>
<br>
Figure 5. Redtail Drone with heatsink and fans.
</p>

The GAAS project provided some baseline SLAM algorithms, but they were written to compile on a CISC machine, and so I had to make several modifications in order to get this working on the RISC based Jetson TX2. This exposed me to Point Cloud Library (PCL) and OpenCV, and taught me about the intrinsic parameters of cameras. 

<p align="center">
<img src='/images/slam.png'>
<br>
Figure 6. Visualizing some of the experiments using YGZ-SLAM and Block Matching Algorithms.
</p>

I  co-authored a publication "Cell A* for Navigation of Unmanned Aerial Vehicles in Partially-Known Environments" for the development of a novel version of Hybrid A* path planning algorithm with Dr. Han and two other graduate students [Wenjian Hao](https://www.linkedin.com/in/wenjianhao/) and [Rongyao "Tony" Wang](https://www.linkedin.com/in/wang-rongyao-268036114/) [3].

The parallels drawn between the drones Robotics Operating System (ROS) packages and the ground vehicles ROS packages made the development of the autonomous systems a collaborative project. During this time, I started to build my leadership and teamwork skills. I organized weekly team meetings and explored autonomous vehicles tech stacks with my team members. Together, we have performed simultaneous localization and mapping (SLAM), sensor fusion using extended Kalman filters (EKF), experimented with different navigation algorithms, human pose recognition, object detection algorithms, and developed deep neural networks for control and disparity map estimation. 

[<img src='/images/ci_vid.png'>](https://www.youtube.com/watch?v=ADZdTsXEJ1I)

References:

[1] Smolyanskiy, Nikolai, et al. “On the Importance of Stereo for Accurate Depth Estimation: An Efficient Semi-Supervised Deep Neural Network Approach.” ArXiv.org, 8 July 2020, arxiv.org/abs/1803.09719.

[2] Smolyanskiy, Nikolai, et al. “Toward Low-Flying Autonomous MAV Trail Navigation Using Deep Neural Networks for Environmental Awareness.” ArXiv.org, 22 July 2017, arxiv.org/abs/1705.02550.

[3] W. Hao, R. Wang, A. Krolicki, and Y. Han, "Cell A* for Navigation of Unmanned Aerial Vehicles in Partially-known Environments" ArXiv.org, 16 September 2020, arxiv.org/abs/2009.07404.

