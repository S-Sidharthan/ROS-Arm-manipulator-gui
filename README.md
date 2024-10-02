# **Robotic Manipulator GUI with AR2 Arm in ROS**

This project implements a ROS-based GUI to control a robotic manipulator using the AR2 arm model. The CAD model was imported into SolidWorks, where the links and joints were defined, then converted to a URDF file. The arm is controlled using the MoveIt package, with real-time motion planning and execution managed via a custom ROS GUI.

## Table of Contents
- [Project Overview](#project-overview)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Images](#images)
- [Video Demo](#video-demo)
- [Contributing](#contributing)

## Project Overview

This project focuses on providing a graphical interface to control the AR2 robotic arm using ROS. The robotic arm's model is defined through a URDF, configured with the MoveIt package for motion planning and control. The GUI allows for intuitive manipulation, offering features such as forward and inverse kinematics, and real-time control of the robotic arm's movements.

## Features
- **URDF Modeling**: The AR2 robotic arm model defined with URDF.
- **MoveIt Integration**: Full MoveIt configuration for motion planning and collision avoidance.
- **ROS GUI**: A user-friendly GUI to control the manipulator's movements.
- **Real-time Visualization**: Real-time visualization and control in RViz.

## Installation

### Prerequisites

Ensure the following dependencies are installed:

- ROS Noetic
- `moveit` package
  ```
  sudo apt-get install ros-noetic-moveit
  ```

### Steps
1. Clone the repository:
```
git clone https://github.com/S-Sidharthan/ROS-Arm-manipulator-gui.git
```

2. Build the project:
```
cd ROS-Arm-manipulator-gui
catkin_make
```

3. Source the workspace:
```
source devel/setup.bash
```

## Usage
Launch MoveIt for AR2 Arm
To launch the MoveIt configuration for the AR2 robotic arm and start controlling the arm using the GUI:
```
roslaunch AR2_Robot_Assembly gazebo.launch 
roslaunch arm_pdg demo.launch 
```


## Images
Figure 1: Robotic arm in gazebo.
![Screenshot from 2024-10-02 19-00-03](https://github.com/user-attachments/assets/88c23394-795f-427c-a2b2-16ebc71da96a)


Figure 2: Real-time visualization in RViz.
![Screenshot from 2024-10-02 19-04-42](https://github.com/user-attachments/assets/514da9cc-b661-4411-8a3c-d4bb6015d080)

## Video Demo

Watch a demo of the robot in action on YouTube:

[https://www.youtube.com/watch?v=iV6wcWm2Lak](https://www.youtube.com/watch?v=iV6wcWm2Lak)

## Contributing
Contributions are welcome! Open issues or submit pull requests to improve the project.
