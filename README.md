TortoiseBot URDF – ROS Jazzy

This repository contains the URDF model and simulation files for TortoiseBot, a mobile robot I designed in Autodesk Fusion 360 and integrated for ROS 2 Jazzy. The package provides everything needed to visualize the robot in RViz, simulate it in Gazebo, and control it using ROS teleoperation tools.

⚠️ This is an independent project — it has no relation to other publicly available TortoiseBot repositories.


📂 Package Contents
<pre> tortoisebot_description/
├── urdf/
│   └── tortoisebot.urdf        # Robot model (from Fusion 360)
├── launch/
│   ├── display.launch.py       # Launch RViz + robot_state_publisher
│   └── gazebo.launch.py        # Launch Gazebo with default world
├── package.xml                 # ROS package manifest
└── CMakeLists.txt              # Build and install setup</pre>


🚀 Features

✅ Complete URDF description of TortoiseBot

✅ Modeled independently in Fusion 360

✅ Runs on ROS 2 Jazzy

✅ Compatible with RViz for visualization

✅ Works in Gazebo for physics-based simulation

✅ Supports teleoperation with teleop_twist_keyboard

✅ Easy to extend with sensors, navigation, and SLAM


🛠️ Installation

Clone the package into your ROS 2 workspace:

<pre>cd ~/ros2_ws/src
git clone https://github.com/yourusername/tortoisebot_description.git
cd ~/ros2_ws
colcon build
source install/setup.bash </pre>


👀 Visualize in RViz

<pre>ros2 launch tortoisebot_description display.launch.py</pre>


🎮 Simulate in Gazebo
1. Launch Gazebo:

<pre>ros2 launch tortoisebot_description gazebo.launch.py</pre>

2. Spawn the robot into Gazebo:

<pre>ros2 run gazebo_ros spawn_entity.py -file src/tortoisebot_description/urdf/tortoisebot.urdf -entity tortoisebot</pre>

3. Run teleoperation:

<pre>ros2 run teleop_twist_keyboard teleop_twist_keyboard</pre>


