cmake_minimum_required(VERSION 2.8.3)
project(ros_screencast)

find_package(catkin REQUIRED)

###################################
## catkin specific configuration ##
###################################
catkin_package(
  DEPENDS python
)

#############
## Install ##
#############
install(PROGRAMS
  scripts/screencast
  DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION}
)
