cmake_minimum_required(VERSION 3.29)
project(lauf_misham_yuna_cpp)

set(CMAKE_CXX_STANDARD 20)

find_package( OpenCV REQUIRED )
include_directories( ${OpenCV_INCLUDE_DIRS} )
add_executable( lauf_misham_yuna_cpp main.cpp
        dnn/common.hpp)
target_link_libraries( lauf_misham_yuna_cpp ${OpenCV_LIBS} )

