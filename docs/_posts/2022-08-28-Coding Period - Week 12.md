---
layout: single
title:  "Coding Period - Week 12"
---
 
We discussed at the beginning of the week, and the task at hand was to migrate all local development packages into a single sdf format, while also starting to incorporate the car model into the RoboticsAcademy Project.
### Migration
I started migrating all the xacro files to the urdf format. There were two ways of going about it, one way was to convert the files directly by rewriting them, which is not really realistic and the other way was to convert them using xacro command and later inspect the URDF to make sure it makes sense.
 
I chose the latter and started the migration process, the xacro error messages can be quite cryptic, especially if there is a non-xml syntax error (such as missing a closing } from ${}. The only remedy I have found is reading carefully and using the text editor to make sure that all braces are matched.
 
Once they have been migrated, gazebo can now directly call the urdf which internally converts it into sdf and the problem is solved.
 
### Environment Variables
 
I started by importing all the local packages into catkin workspace inside the RADI, everything was good even after the catkin build, so what was stopping me from adding launch instructions in the instructions.json file to start launching the exercise?
 
Every Instance of ssh opens a new terminal having its own environment variables and updating the env variables inside one terminal will not change the state of them in the current RADI Instance. The packages would run perfectly inside RADI after catkin build inside the terminal where it was build but not outside of that particular shell.
 
So the main problem at root was to import all packages into Docker File and build them.
 
### Tasks
- [x] Migrate all packages under one sdf format.
 
### Conclusion
Although there were a lot of dependency errors while building on DockerFile a certain progress has been made to eliminate a few, the next week will be more concentrated towards solving all the dependency issues and building the DockerFile with the car models.