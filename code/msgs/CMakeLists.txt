cmake_minimum_required(VERSION 2.8.3)
project(hal_msgs)

## Find catkin macros and libraries
find_package(catkin REQUIRED
  genmsg
  std_msgs
  sensor_msgs
  geometry_msgs
)

# Generate messages in the 'msg' folder
add_message_files(
  DIRECTORY msg
  FILES
  speed_pair.msg
)

# Generate added messages and services with any dependencies listed here
generate_messages(
  DEPENDENCIES
  std_msgs
)

catkin_package()
