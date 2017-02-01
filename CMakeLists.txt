cmake_minimum_required(VERSION 2.8)

project( caltest C CXX )

set(COMPILE_DEFINITIONS -Werror)

#set(CMAKE_VERBOSE_MAKEFILE TRUE)
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -lstdc++")

find_package(OpenCV REQUIRED)

add_executable(caltest calibrate.cpp)

target_link_libraries( caltest ${OpenCV_LIBS} )

