cmake_minimum_required(VERSION 3.0.2)
project(turtlebot3_msgs)

find_package(catkin REQUIRED COMPONENTS
  std_msgs
  message_generation
)

add_message_files(
  FILES
  SensorState.msg
  Sound.msg
  VersionInfo.msg
)

generate_messages(
  DEPENDENCIES
  std_msgs
)

catkin_package(
  CATKIN_DEPENDS message_runtime std_msgs
)

