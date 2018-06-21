cmake_minimum_required(VERSION 2.8.3)
project(blockly)

find_package(catkin REQUIRED COMPONENTS rospy std_msgs)

catkin_package(CATKIN_DEPENDS std_msgs)

catkin_install_python(PROGRAMS
  scripts/blockly_backend.py
  DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION}/scripts
)
