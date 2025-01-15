cmake_minimum_required(VERSION 2.8.3)
project(go2_config)

find_package(catkin REQUIRED COMPONENTS
  roscpp
  std_msgs
  sensor_msgs
  tf
)

catkin_package()

install(DIRECTORY config launch meshes urdf maps worlds
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)