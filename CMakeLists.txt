cmake_minimum_required(VERSION 3.0)
project(OpenCV_test)
set(CMAKE_CXX_STANDARD 14)

find_package(OpenCV REQUIRED)

include_directories(${OpenCV_INCLUDE_DIRS} src)
add_executable(opencv_test src/main.cpp)
target_link_libraries(opencv_test ${OpenCV_LIBS})
