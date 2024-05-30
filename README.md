# ur5_moveit_demonstration
Project Overview
This project is created to demonstrate ROS MoveIt configuration. Here, I used the UR5 robotic arm and Robotiq 85 gripper. The project scope is to pick an object located at a predefined location and place it in a predefined target position while avoiding collisions. The robot can avoid collisions in unknown environments and even react to changes in its surroundings using a depth camera.

Requirements
For this work, you need to install the Universal Robot Industrial package. Clone the Universal Robots repository (this is developed for ROS Kinetic).

bash
Copy code
~/catkin_ws/src$ git clone https://github.com/ros-industrial/universal_robot.git
Package Description
The ur5_simple_pick_and_place package is created to pick an object from a defined location and place it in a target position.

How to Run
Launch the demo in Gazebo:

bash
Copy code
$ roslaunch ur5_moveit_config demo_gazebo.launch
Run the pick and place node:

bash
Copy code
$ rosrun ur5_simple_pick_and_place pick_and_place_collision_depth_camera
