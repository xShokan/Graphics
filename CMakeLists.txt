cmake_minimum_required(VERSION 3.31)
project(Graphics)

set(CMAKE_CXX_STANDARD 20)

add_executable(Graphics src/glad.c main.cpp)
include_directories(include)
link_directories(lib)

target_link_libraries(Graphics ${PROJECT_SOURCE_DIR}/lib/GLFW/glfw3.lib)
