cmake_minimum_required(VERSION 2.8)
project (work5orb)
set (CMAKE_CXX_FLAGS "${CMAKE_CXX_FALGS} -std=c++11")
find_package (OpenCV 3.3.0 REQUIRED)
INCLUDE_DIRECTORIES(${OpenCV_INCLUDE_DIRS})
ADD_EXECUTABLE( ORB computeORB.cpp)
target_link_libraries (ORB ${OpenCV_LIBS})

