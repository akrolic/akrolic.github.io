---
title: "Dynamic Systems Class Project: Frequency Analysis and System Response of a 1/18th Scale Race Car (AWS DeepRacer)"
excerpt: "<br/><img src='/images/500x300.png'>"
collection: portfolio
---

------

[Final Project Report](/files/ME3050 Project Report.pdf) | [Supplemental Video](https://express.adobe.com/video/byEgTq6KgdgB1)

Abstract:

The amazon DeepRacer is an autonomous race car designed to aid developers and students in learning how to implement artificial intelligence through reinforcement learning on a 1/18th scale race car. The all-wheel drive vehicle is equipped with an independent double wishbone front suspension with coilover shock absorbers. A servomotor is used to move the front tie-rods and control steering. The independent rear suspension resembles the NASCAR truck-arm style lower control arm configuration coupled with a coilover shock absorber. The vehicle has rubber tires that carry their own stiffness and dampening coefficients. The RC car is capable of reaching incredible speeds, however these speeds do not need to be achieved in order to analyze the response of the system. 

<p align="center">
<img src='/images/deep_racer.png'>
<br>
Figure 1. AWS DeepRacer Chassis and Suspension Configuration.
</p>

Objectives
* Create various test tracks to simulate an input on the vehicles suspension and record the accelerations using an accelerometer from the NI-MyRIO data acquisition system. 
* Integrate the accelerometer data and determine the displacement of the vehicle.
* Determine the approximate stiffness of the coilovers by taking measurements of the vehicle’s springs under known loads.
* Using the accelerometer data find the systems approximate stiffness and dampening coefficients using logarithmic decent or by measuring the maximum overshoot.
* Find the approximate tire stiffness.
* Create a sinusoidal track designed based on the approximate values of [m,c,k] then evaluate the theoretical response of the system to the actual response. 
* Fine tune the parameters to determine a best fit of the system. 

Project Summary: 

The objective of this project is to preform experiments, gather data and model the vehicles suspension for future development of a control algorithm that would enhance the vehicles autonomous driving capabilities. Currently the car only utilizes image processing techniques to make steering and throttle decisions. The motivation for gathering this data is to create a model that approximates the response of the suspension, so that it can be incorporated into the simulation which will learn over several thousand iterations around a track. The cars goal is to complete laps around a track as fast as possible and leveraging the accelerometer data to push the car harder around corners will aid in achieving this goal.


