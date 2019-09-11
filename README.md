# Shallow-Depth Insertion (Deprecated)

***Note: This package has been deprecated. To see the most recent version, go [here](https://github.com/HKUST-RML/shallow_depth_insertion).***

This is a ROS package to demonstrate a robotic manipulation technique, particularly assembling a thin object into a complementary shallow hole. The utilized hardware includes UR10 robotic arm and Robotiq 2-Finger 140mm Adaptive parallel-jaw gripper. 

To watch video, see: [here](https://www.youtube.com/watch?v=Nka-sCzrcSs)

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Hardware Prerequisites
- Universal Robots UR10 robot arm

- Robotiq 140mm Adaptive parallel-jaw gripper

- FT 300 Force Torque Sensor

- 1080p webcam 

### Software Prerequisites
- ROS kinetic 
- [universal_robot package](http://wiki.ros.org/universal_robot)
- [ur_modern_driver](https://github.com/ThomasTimm/ur_modern_driver)
- [MoveIt!](http://docs.ros.org/kinetic/api/moveit_tutorials/html/index.html) 
- Rviz
- Software tested on Ubuntu 16.04.3 LTS.
- AprilTags

## How to run it

1. Appropriately connect to the robot arm and gripper hardwares. 
2. Launch 
```
roslaunch shallow_depth_insertion manipulation_ur10.launch
```
```
roslaunch shallow_depth_insertion april_tags.launch
```
3. Run the executable python script:
```
rosrun shallow_depth_insertion shallow_depth_insertion.py
```

## Authors

* **John Kim** (chkimaa@connect.ust.hk)

