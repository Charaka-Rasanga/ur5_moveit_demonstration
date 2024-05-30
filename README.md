# ur5_moveit_demonstration
Project Overview:

This project is created to demonstrate ROS MoveIt configuration. Here, I used the UR5 robotic arm and Robotiq 85 gripper. The project scope is to pick an object located at a predefined location and place it in a predefined target position while avoiding collisions. The robot can avoid collisions in unknown environments and even react to changes in its surroundings using a depth camera.

Here is a link to an example video that I posted on my LinkedIn profile: https://www.linkedin.com/posts/charaka-rasanga-b1350241_ros-moveit-octomap-collision-avoiding-and-activity-6981609869086781441-NzGN?utm_source=share&utm_medium=member_desktop

Requirements:

For this work, you need to install the Universal Robot Industrial package. Clone the Universal Robots repository (this is developed for ROS Kinetic).


Copy code:

~/catkin_ws/src$ git clone https://github.com/ros-industrial/universal_robot.git
Package Description
The ur5_simple_pick_and_place package is created to pick an object from a defined location and place it in a target position. That was   implemented using C++.

How to Run:

Launch the demo in Gazebo:


Copy code:

$ roslaunch ur5_moveit_config demo_gazebo.launch

Run the pick and place node:

Copy code:

$ rosrun ur5_simple_pick_and_place pick_and_place_collision_depth_camera
