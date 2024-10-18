cmake_minimum_required(VERSION 3.20)
set(PROJECT sangam)
set(CMAKE_EXPORT_COMPILE_COMMANDS ON)
project(${PROJECT} C CXX)

file(GLOB SOURCES
  ${CMAKE_SOURCE_DIR}/src/*.cpp 
)

include_directories(
  ${CMAKE_SOURCE_DIR}/include/ 
)

add_executable(${PROJECT} ${SOURCES})

