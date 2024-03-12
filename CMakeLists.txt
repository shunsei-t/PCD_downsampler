cmake_minimum_required(VERSION 3.5 FATAL_ERROR)

project(pcd_downsampler)

find_package(PCL 1.2 REQUIRED)

include_directories(${PCL_INCLUDE_DIRS})
link_directories(${PCL_LIBRARY_DIRS})
add_definitions(${PCL_DEFINITIONS})

add_executable (pcd_downsampler main.cpp)
target_link_libraries (pcd_downsampler ${PCL_LIBRARIES})