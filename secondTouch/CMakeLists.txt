cmake_minimum_required(VERSION 3.10)
project(secondTouch)

set(CMAKE_CXX_STANDARD 11)

set(SOURCE_FILES main.cpp)

include_directories(${PROJECT_SOURCE_DIR}/../GLFW/inc)

link_directories(${PROJECT_SOURCE_DIR}/../GLFW/lib-mingw-w64)

add_executable(secondTouch ${SOURCE_FILES})

target_link_libraries(secondTouch glfw3 gdi32 opengl32)