cmake_minimum_required(VERSION 3.0.2)
project(lidar_replay)

find_package(catkin REQUIRED COMPONENTS
  ouster_ros
  velodyne_pointcloud
)

###################################
## catkin specific configuration ##
###################################
catkin_package()

#############
## Install ##
#############
install(DIRECTORY launch
        DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION})

install(DIRECTORY params
DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION})