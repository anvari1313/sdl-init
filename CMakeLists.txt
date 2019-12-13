cmake_minimum_required(VERSION 3.15)
project(sdltest)

set(CMAKE_CXX_STANDARD 17)

find_package(SDL2 REQUIRED)
include_directories(${SDL2_INCLUDE_DIRS})

add_executable(sdltest main.cpp)

target_link_libraries(sdltest ${SDL2_LIBRARIES})