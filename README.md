# Hospital-Service-Robot-Simulation-_Human-Robot-Interactions
ROS Noetic + Gazebo 11 simulation of a 4x scaled TurtleBot3 in a custom hospital world with keyboard teleoperation and controller customization.


This project simulates a **4x scaled TurtleBot3** in a custom Gazebo hospital environment (`oda4_with_keyboard_control.world`).

## Features
- ✅ 4x enlarged TurtleBot3 (custom URDF)
- ✅ Custom Gazebo world
- ✅ Keyboard control via teleop
- ✅ Custom wheel/control parameters

## How to Run

```bash
source devel_isolated/setup.bash
export TURTLEBOT3_MODEL=burger
roslaunch my_worlds spawn_turtlebot_in_oda4.launch

In another terminal:

source devel_isolated/setup.bash
export TURTLEBOT3_MODEL=burger
roslaunch turtlebot3_teleop turtlebot3_teleop_key.launch

