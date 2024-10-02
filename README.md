**Robotic Manipulator GUI with AR2 Arm in ROS**
This project implements a ROS-based GUI to control a robotic manipulator using the AR2 arm model. The CAD model was imported into SolidWorks, where the links and joints were defined, then converted to a URDF file. The arm is controlled using the MoveIt package, with real-time motion planning and execution managed via a custom ROS GUI.

Table of Contents
Project Overview
Features
Installation
Usage
Images
Contributing
License
Project Overview
This project focuses on providing a graphical interface to control the AR2 robotic arm using ROS. The robotic arm's model is defined through a URDF, configured with the MoveIt package for motion planning and control. The GUI allows for intuitive manipulation, offering features such as forward and inverse kinematics, and real-time control of the robotic arm's movements.

Features
URDF Modeling: The AR2 robotic arm model defined with URDF.
MoveIt Integration: Full MoveIt configuration for motion planning and collision avoidance.
ROS GUI: A user-friendly GUI to control the manipulator's movements.
Real-time Visualization: Real-time visualization and control in RViz.
Installation
Prerequisites
Ensure the following dependencies are installed:

ROS
moveit package
ros_control package
RViz
Steps
Clone the repository:

git clone https://github.com/yourusername/yourmanipulatorproject.git
Build the project:

cd yourmanipulatorproject
catkin_make
Source the workspace:

source devel/setup.bash
Usage
Launch MoveIt for AR2 Arm
To launch the MoveIt configuration for the AR2 robotic arm and start controlling the arm using the GUI:

sudo apt-get install ros-noetic-moveit
roslaunch AR2_Robot_Assembly gazebo.launch 
roslaunch arm_pdg demo.launch 


Control via GUI
Use the custom ROS GUI to control the robotic manipulator’s movements. The GUI supports:

Forward Kinematics: Control each joint directly.
Inverse Kinematics: Define the end-effector’s desired position and orientation.
Rviz Visualization
To visualize the robotic arm’s movements:

roslaunch yourpackage rviz_arm.launch
Images
Figure 1: GUI for controlling AR2 robotic arm.

Figure 2: Real-time visualization in RViz.

Contributing
Contributions are welcome! Open issues or submit pull requests to improve the project.
