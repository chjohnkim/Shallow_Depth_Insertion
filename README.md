# Shallow-Depth Insertion

This is a ROS package to demonstrate a robotic manipulation technique, particularly assembling a thin object into a complementary shallow hole. The utilized hardware includes UR10 robotic arm and Robotiq 2-Finger 140mm Adaptive parallel-jaw gripper. 

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Hardware Prerequisites
#### Universal Robots UR10 robot arm

#### Robotiq 140mm Adaptive parallel-jaw gripper

#### FT 300 Force Torque Sensor

#### 1080p webcam 

### Software Prerequisites
- ROS kinetic 
- universal_robot package [link](http://wiki.ros.org/universal_robot)
- ur_modern_driver [link](https://github.com/ThomasTimm/ur_modern_driver)
- MoveIt! [link](http://docs.ros.org/kinetic/api/moveit_tutorials/html/index.html) 
- Rviz
- Software tested on Ubuntu 16.04.3 LTS.

## How to run it

1. Run a gazebo simulation by launching the following commands in three different terminals
```
roscore
```
```
roslaunch ur_gazebo ur10.launch
```
```
roslaunch ur10_moveit_config ur10_moveit_planning_execution.launch sim:=true
```
2. Rviz can also be executed with the following command on a fourth terminal
```
roslaunch ur10_moveit_config moveit_rviz.launch config:=true
```
3. Run the executable python motion plan to run simulation in gazebo environment:
```
rosrun ur10_motion_script ur10_turnArcFunction.py
```
OR just launch a launch file
```
roslaunch ur10_motion_script simulation.launch
```

## Authors

* **John Kim** 

