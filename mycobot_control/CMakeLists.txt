cmake_minimum_required(VERSION 3.0.2)
project(mycobot_control)

find_package(catkin REQUIRED)

catkin_package()

install(DIRECTORY config launch
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)
