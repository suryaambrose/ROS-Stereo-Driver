cmake_minimum_required(VERSION 2.8.3)
project(stereo_driver)

## Find catkin macros and libraries
## if COMPONENTS list like find_package(catkin REQUIRED COMPONENTS xyz)
## is used, also find other catkin packages
find_package(catkin REQUIRED COMPONENTS roscpp camera_info_manager dynamic_reconfigure image_transport nodelet sensor_msgs cv_bridge)

find_package(OpenCV REQUIRED COMPONENTS core highgui imgproc)
if (OpenCV_VERSION VERSION_EQUAL "3")
  add_definitions("-DOPENCV3=1")
endif()

catkin_package(
  CATKIN_DEPENDS
    roscpp
    camera_info_manager
    dynamic_reconfigure
    image_transport
    nodelet
    sensor_msgs
    cv_bridge
  )