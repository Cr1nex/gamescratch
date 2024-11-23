cmake_minimum_required(VERSION 3.10)
project(SDL2_Project)

set(CMAKE_CXX_STANDARD 17)

find_package(SDL2 REQUIRED)
include_directories(${SDL2_INCLUDE_DIRS})

add_executable(sdl2_example main.cpp)
target_link_libraries(sdl2_example ${SDL2_LIBRARIES})