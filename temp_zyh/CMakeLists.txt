cmake_minimum_required(VERSION 3.20.0)

#项目名
set(PROJECT_NAME temp)

#项目名设置
project(${PROJECT_NAME})

#设计c++标准版本
set(CMAKE_CXX_STANDARD 11)

set(CMAKE_BUILD_TYPE "Debug")

add_subdirectory(src)

add_subdirectory(test)

target_link_libraries(test src)