cmake_minimum_required(VERSION 2.8.3)
project(launch_files)

find_package(catkin REQUIRED)

catkin_package(
    INCLUDE_DIRS
    LIBRARIES
    CATKIN_DEPENDS
    DEPENDS
    )

install(DIRECTORY launch/
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}/launch)

install(DIRECTORY config/
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}/config)
