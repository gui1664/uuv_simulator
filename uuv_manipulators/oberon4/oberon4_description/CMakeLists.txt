cmake_minimum_required(VERSION 2.8.3)
project(oberon4_description)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")

find_package(catkin)

catkin_package()

install(DIRECTORY meshes params robots urdf
        DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
        PATTERN "*~" EXCLUDE)
