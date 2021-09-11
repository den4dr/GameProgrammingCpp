cmake_minimum_required(VERSION 3.20)
project(GameProgrammingCpp)

set(CMAKE_CXX_STANDARD 23)

find_package(SDL2 CONFIG REQUIRED)
add_executable(GameProgrammingCpp Main.cpp Game.h Game.cpp)

target_link_libraries(GameProgrammingCpp PRIVATE SDL2::SDL2 SDL2::SDL2main SDL2::SDL2-static)