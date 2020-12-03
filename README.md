# rse-nd-project-3
Course project "Where Am I" repository for the Udacity Robotics Software Engineer Nanodegree program.

This project contains the following Catkin packages :
* renato_robot: 
    * Implementation of a differential drive robot with lidar sensor and camera, written in URDF.
    * Contains a world called `restaurant_renato.world`.
    * Contains a `rviz_amcl.rviz` file with a preset of rviz configs for this project.
    * Launch files
        * `amcl.launch`: amcl node.
        * `world.launch`: gazebo world and spawn robot.

Screenshots folder where included with screens hots of each part of the amcl simulation and converging to robot's real position.

## Installation
Clone this repository in **src** folder in your catkin workspace and following repositories bellow:
```
cd ~/catkin_ws/src
git clone https://github.com/rodriguesrenato/rse-nd-project-3.git
cd rse-nd-project-3
git clone https://github.com/ros-teleop/teleop_twist_keyboard
git clone https://github.com/udacity/pgm_map_creator.git
```


## Usage
Supposing your catkin workspace is located in ~/
```
cd ~/catkin_ws
catkin_make
source devel/setup.bash
```
Use the .launch files to launch packages.
* Terminal 1: `roslaunch renato_robot world.launch`
* Terminal 2: `roslaunch renato_robot amcl.launch`
* Terminal 3: `roslaunch renato_robot rviz_amcl.launch`
* Terminal 4:  `rosrun teleop_twist_keyboard teleop_twist_keyboard.py`

## License
The contents of this repository are covered under the MIT License.
