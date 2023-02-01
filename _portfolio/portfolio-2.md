---
title: "CAST - Unmanned Aerial Vehicles (UAV)"
excerpt: "<br/><img src='/images/Drones.jpg'>"
collection: portfolio
---

When I was a undergraduate student in Spring 2018, [Dr. Yiqiang Han](https://www.clemson.edu/cecas/departments/me/people/faculty/han.html) invited me to join his undergraduate research group who was focused on building, developing, and testing unmanned aerial vehicles. At that time, [Duncan Nicholson](https://www.linkedin.com/in/duncanicholson/) was the team lead, and he taught me all of the fundamentals of ROS, linux, and the hardware associated with the drone. 

Our team began our journey into the autonomous drone world by experimenting with the [Intel Aero](https://docs.px4.io/main/en/complete_vehicles/intel_aero.html), an out of the box solution that allowed our team to hit the ground running on learning new techniques and algorithms on a capable computing platform. We eventually retired the development of the Aero Drone due to its limitations and restrictions in pursuing more open source solutions.

Our first in house drone was designed to compete in the Vertical Flight Societies (VFS) [7th Annual MAV Student Challange](https://vtol.org/education/micro-air-vehicle-student-challenge/micro-air-vehicle-student-challenge-2019). The competition required that we construct a micro autonomous drone(<500g) to navigate and complete an indoor course with a variety of objectives to complete such as picking up a payload and dropping it off at a designated location. These technical challanges, combined with the hardware limitations at the time, made this difficult for us to complete the qualifying requirements in time to attend the event. This was also the first year of our research group's experience in building autonomous systems. It was a great learning exercise and motivation for all of us and in the end we built our first edge autonomous drone using the NVIDIA TX2 smacked on top of a px4 racer flight controller. 

<p align="center">
<img src='/images/muav.jpg'>
<br>
Figure 1. Micro autonomous drone - designed for the 7th Annual MAV Student Challange. 
</p>



I was the team lead in developing autonomous control algorithms for both the drone and race car projects. The parallels drawn between the drones Robotics Operating System (ROS) packages and the ground vehicles ROS packages made the development of the autonomous systems a collaborative project. During this time, I started to build my leadership and teamwork skills. I organized weekly team meetings and explored autonomous vehicles tech stacks with my team members. Together, we have performed simultaneous localization and mapping (SLAM), sensor fusion using extended Kalman filters (EKF), experimented with different navigation algorithms, human pose recognition, object detection algorithms, and developed deep neural networks for control and disparity map estimation. I recently co-authored in a publication "Cell A* for Navigation of Unmanned Aerial Vehicles in Partially-Known Environments" for my work in the development of a novel version of Hybrid A* path planning algorithm with Dr. Han and two other graduate students.

References:

[1] Smolyanskiy, Nikolai, et al. “On the Importance of Stereo for Accurate Depth Estimation: An Efficient Semi-Supervised Deep Neural Network Approach.” ArXiv.org, 8 July 2020, arxiv.org/abs/1803.09719.

[2] Smolyanskiy, Nikolai, et al. “Toward Low-Flying Autonomous MAV Trail Navigation Using Deep Neural Networks for Environmental Awareness.” ArXiv.org, 22 July 2017, arxiv.org/abs/1705.02550.

[3] W. Hao, R. Wang, A. Krolicki, and Y. Han, "Cell A* for Navigation of Unmanned Aerial Vehicles in Partially-known Environments" ArXiv.org, 16 September 2020, arxiv.org/abs/2009.07404.

