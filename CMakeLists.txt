cmake_minimum_required(VERSION 3.12)
project(template)

FILE(GLOB_RECURSE SOURCES src/*.cpp)
add_executable(template ${SOURCES})
target_include_directories(template PRIVATE include)

set(CMAKE_EXPORT_COMPILE_COMMANDS ON)
install(TARGETS template)