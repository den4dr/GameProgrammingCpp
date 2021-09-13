cmake_minimum_required(VERSION 3.20)
project(chapter01)

set(CMAKE_CXX_STANDARD 23)

find_package(SDL2 CONFIG REQUIRED)

add_executable(chapter01 main.cpp Game.cpp Game.h)

target_link_libraries(chapter01 PRIVATE SDL2::SDL2 SDL2::SDL2main)
