cmake_minimum_required(VERSION 3.25)
project(OpenGLTest)

set(CMAKE_CXX_STANDARD 17)

add_executable(${PROJECT_NAME} main.cpp glad.c)

include_directories("GLFW/include")

target_link_libraries(OpenGLTest "${CMAKE_SOURCE_DIR}/GLFW/libs/glfw3.lib")
