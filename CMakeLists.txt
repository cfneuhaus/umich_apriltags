cmake_minimum_required(VERSION 3.0)
project(umich_apriltags)

set(CMAKE_EXPORT_COMPILE_COMMANDS "ON")

file(GLOB SOURCES *.c *.h  common/*.c common/*.h)
add_library(umich_apriltags ${SOURCES})
target_include_directories(umich_apriltags PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})
