---
layout: single
title:  "Coding Period - Week 7"
---
We had a discussion at the beginning of the week, the task at hand was to get improve asthetics and also add a camera module to thee front of the Lincoln Mkz car.
 
### The Camera module lag 😔

A camera module is very important to a self-driving car and what's more important is a latency-free camera module. I started by adding a camera module to the Lincoln Mkz and what resulted was a very good quality codec output but what followed was the latency in frames received. This latency could cause a delay in actions performed by the car and that will take a huge toll on the performance.
 
One way to decrease this latency is to compress the images and have a specific topic publish the compressed frames, **[Compressed_image_transport](http://wiki.ros.org/compressed_image_transport)** package is one such package which does this job well.
 
After compressing the camera images the latency issue is solved 😊.

### How did I upgrade the Textures

It's very important for a simulation model to look realistic, a realistic model is what encourages anyone to code in a simulation mode.
 
I started by adding and testing out different color and textures to the car model in **Fusion 360** and it was a big mistake as I realized fusion 360 does not export colors when exported as urdf.
 
After a little research I found out that **Blender** is one such tool where this does not happen, so I applied all the changes I previously made inside blender.
 
Now the Car is as good as it gets!
 
 
### Tasks
- [x] Upgrade Lincoln-mkz Car model with better Textures.
- [x] Add a Camera Module to capture the front view of the car.
 
## Progress Video
 
{% include video id="mlFsR78OP7A" provider="youtube" %}