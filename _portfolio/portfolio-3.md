---
title: "CAST - Unmanned Ground Vehicles (UGV)"
excerpt: "<br/><img src='/images/AGV.jpg'>"
collection: portfolio
---

The Clemson Autonomous Systems Team gitbook documentation can be accessed [here](https://clemson-autonomous-systems.gitbook.io/clemson-university-autonomous-systems/), a summary of my contributions and collaberations are given below. 

When I was a undergraduate student in Spring 2019, [Dr. Yiqiang Han](https://www.clemson.edu/cecas/departments/me/people/faculty/han.html) asked me to lead his undergraduate research group who was focused on building, developing, and testing unmanned ground vehicles. At that time, [Wenjian Hao](https://www.linkedin.com/in/duncanicholson/) was a graduate student advising our project, and he taught me all of the fundamentals of Reinforcement Learning and Deep Learning. 

Our first autonomous ground vehicle was the AWS DeepRacer, which at that time was just released to academia for testing. The DeepRacer was an end-to-end learning platform, where training was completed in a virtual environment and then the learned policy was deployed onto the vehicle. This platform was a great way to quickly get hands on experience performing real2sim policy transfer, we even built a to scale track and showcased our work at the 2019 FoCI event at Clemson University. 

<p align="center">
<img src='/images/deepracer_foci.png'>
<br>
Figure 1. FoCI 2019 event showcasing the AWS DeepRacer. 
</p>

Ultimately our findings from this exercise were underwhelming, we learned the limitations of Deep Reinforcement Learning, and the challanges associated with transfering a policy from simulation to the vehicle. 

A majority of my experience with autonomous ground vehicles was in simulation using the [F1TENTH]() simulation platform. Our team was advised by graduate student [Rongyao "Tony" Wang](https://www.linkedin.com/in/wang-rongyao-268036114/), and together we competed in two virtual F1TENTH competitions. 

<p align="center">
<img src='/images/f1tenth_certs.png'>
<br>
Figure 2. F1TENTH competition certificates. 
</p>

Eventually, we wanted to test multi-agent algorithms and decided to experiment with a tracked vehicle rather than an ackermann steer vehicle. At this point, we were developing from our apartments, and I was working with very few resources but still was able to take an old shoe box, paint it orange and outfit a scaled tank with a 2D lidar, xbee, and stereo camera to test out multi-agent mapping algorithms. 

<p align="center">
<img src='/images/tank_pic.jpg'>
<br>
Figure 3. Pandemic Tank. 
</p>

This work was completed with [Jonathan Daniel](https://www.linkedin.com/in/jonathandaniel23/) and he was able to get great results summarized in his write up [here](https://clemson-autonomous-systems.gitbook.io/clemson-university-autonomous-systems/multi-agent-development).

<p align="center">
<img src='/images/multi-agent.png'>
<br>
Figure 4. Multi-agent mapping diagram with gazebo TurtleBot example. 
</p>

I helped perform the physical testing for [Rongyao "Tony" Wang](https://www.linkedin.com/in/wang-rongyao-268036114/) thesis ["Data-driven System Identification and Optimal Control Framework for Grand-Prix Style Autonomous Racing"](https://tigerprints.clemson.edu/all_theses/3601/)" and was kindly acknowledged [2]. Tony's work was recognized at the 2021 ICRA conference and won the best paper award [1].

[<img src='/images/tony_racer.png'>](https://www.youtube.com/watch?v=ofdRW21QoU4)

Work in progress...

Multiple events and competitions have recognized my research work. My team participated in the F1TENTH International Federation of Controls Conference virtual head-to-head autonomous racing competition in the summer of 2020 and placed in the top 5 in our first year. I worked with my teammates to build our own prototype ground vehicles for deploying and validating the performance of our algorithms using powerful onboard computers with GPU accelerated programs. I helped our team in every stage of development and taught new members how to get started with little to no background experience. We formed the Clemson University Autonomous Systems Team (CAST) and participated in the Clemson Covid Challenge, where we proposed a multi-agent autonomous delivery solution that won the Clemson Covid Challenge Excellence Prize. Our work was selected to be a finalist for South Carolina's InnoVision Award in the Covid-19 Response category.

[1] R. Wang, Y. Han, and U. Vaidya, “Deep Koopman data-driven control framework for Autonomous racing,” in Proc. Int. Conf. Robot.
Autom. (ICRA) Workshop Opportunities Challenges Auton. Racing, 2021, pp. 1–6. [Online]. Available: https://linklab-uva.github.io/icraautonomous-racing/contributed_papers/paper12.pdf

[2] Wang, Rongyao, "Data-driven System Identification and Optimal Control Framework for Grand-Prix Style Autonomous Racing" (2021). All Theses. 3601.