cmake_minimum_required(VERSION 3.22)
project(GameOfLife_DT)

set(CMAKE_CXX_STANDARD 23)

find_package(OpenGL REQUIRED)
find_package(GLEW REQUIRED)
find_package(glfw3 REQUIRED)
set(EXECUTABLE GameOfLife_DT)

add_executable(${EXECUTABLE} main.cpp)

target_link_libraries(${EXECUTABLE} OpenGL::GL)
target_link_libraries(${EXECUTABLE} GLEW::GLEW)
target_link_libraries(${EXECUTABLE} glfw)
