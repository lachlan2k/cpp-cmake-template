cmake_minimum_required(VERSION 3.7)

project(example-project)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_C_STANDARD 11)

include_directories(include)

file(GLOB_RECURSE CXX_SOURCES "src/*.cpp")
file(GLOB_RECURSE C_SOURCES "src/*.c")

add_executable(example-project ${CXX_SOURCES} ${C_SOURCES})