---
layout: single
title:  "Coding Period - Week 9, Week 10"
---
 We discussed at the beginning of the week, that the task at hand was to integrate a 3D Lidar and GPS Sensor while also starting to incorporate the car model into the RoboticsAcademy Project.
 
### 3D Lidar ⚡
A 3D Lidar has been added to the car model, which can now be accessed as a 3-dimensional array, which the user can go on to narrow down as per their Field of View requirement.
 
### The GPS Sensor 🚗
As an addition to the existing Sensors, we have also decided to add a GPS Sensor. This can later be used to create future exercises. The GPS follows the earth model, 1 degree of latitude is 60 arc minutes with one arc minute being up to 1.82 kilometers. Hence, a movement of a few meters will be only a tiny fraction of a degree of latitude or longitude. Hence the user will also need to multiply a proportional constant to the GPS Coordinates to track or notice changes during minute car travel.
 
### Tasks
- [x] Add GPS Sensor to the Lincoln Mkz Model.
- [x] Add a 3D Lidar Module to the Lincoln Mkz Model.
- [x] Add Documentation to Robotics Academy for Developers.
- [x] Start Progress on Implementing Car Model into Car Junction Exercise.
 
### Conclusion
 
Although it was tough to get started on integrating the car model into RADI, coming weeks will be focussed on the integration part while also tailoring the car model to the exercise needs.
 
## Progress Video
 
#### 3D Lidar
{% include video id="k_psCmHe9Ho" provider="youtube" %}
 
#### GPS Sensor
![New Blocks]({{ site.baseurl }}/assets/images/gps.png){: .align-center}