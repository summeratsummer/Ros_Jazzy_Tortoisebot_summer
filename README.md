TortoiseBot URDF – ROS Jazzy

This repository contains the URDF model and simulation files for TortoiseBot, a mobile robot I designed in Autodesk Fusion 360 and integrated for ROS 2 Jazzy. The package provides everything needed to visualize the robot in RViz, simulate it in Gazebo, and control it using ROS teleoperation tools.

⚠️ This is an independent project — it has no relation to other publicly available TortoiseBot repositories.

📂 Package Contents

tortoisebot_description/
├── urdf/
│   └── tortoisebot.urdf        # Robot model (from Fusion 360)
├── launch/
│   ├── display.launch.py       # Launch RViz + robot_state_publisher
│   └── gazebo.launch.py        # Launch Gazebo with default world
├── package.xml                 # ROS package manifest
└── CMakeLists.txt              # Build and install setup
