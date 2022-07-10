---
layout: single
title:  "Coding Period - Week 6"
---
 
The Toyota Car has achieved the full  Ackermann steering and movement needed to be an Autonomous car, but there was still something quite awry with it.
 
### So what went wrong 😔?
 
The packages and hybrid plugins of the Toyota Car were never maintained after the ROSCON '17 Event, this was the time ROS as a framework had most changes to it. ROS Kinetic, which the Toyota Car was presented with went on to become ROS Melodic and then the currently used version to develop this project i.e ROS Noetic.
 
so to bring the Toyota Car to life a lot of dependencies and plugins had to be changed, when a dependency is changed the underlying code still remains the same and just uses the updated dependency to compile the code.
 
That was the problem in the case of our Toyota car model, well coming so far from a model that doesn't work, I wasn't going to leave it without a try. I geared up to solve all the errors the package had. Started from changing message types, plugins to joint state publishers.
 
**QT4 THE DEAD END 🛑...**
 
The underlying code had a QT4 dependency, one way of going about it is to assume none of the changes after QT5 would break the existing code. I started by changing the requirement dependency and the code did not compile, this only meant changing 100s of lines of code and adding to that was the missing QtCreator Docs that were needed for migration.
 
It meant only one thing, coming up with a new model, while I was at this there was always a Plan B. It was the **Lincoln MKZ Model**.
 
Things were quite straight forward from here, working with the Totota Car Model made it easy to deal with the Lincoln MKZ.


### Tasks
- [x] Create a New Car Model.
- [x] Car Model should have Ackermann Physics with movable and turnable wheels replicating a real world car.
- [x] Modular code to add Sensors in future.

## Conclusions

Although it took a lot of time in making this possible the Lincoln MKZ model is sharp at looks and has even better physics compared to the Toyota Prius Model. It definitely stands as an upgrade to the Toyota Prius Model. 

## Progress Video

{% include video id="CW2ddqtC-QY" provider="youtube" %}