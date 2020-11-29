# rse-nd
Course project "Where Am I" repository for the Udacity Robotics Software Engineer Nanodegree program.

This project contains the following Catkin packages :
* renato_robot: Implementation of a differential drive robot with lidar sensor and camera, written in URDF. Contains a world called `restaurant_renato.world`
* project1: A restaurant gazebo world made for Project 1.

## Installation
Clone this repository in **src** folder in your catkin workspace
```
cd ~/catkin_ws/src
git clone https://github.com/rodriguesrenato/rse-nd.git
```
## Usage
Supposing your catkin workspace is located in ~/
```
cd ~/catkin_ws
catkin_make
source devel/setup.bash
```
Use the .launch files to launch packages.
```
roslaunch renato_robot world.launch
```

## License
The contents of this repository are covered under the MIT License.
