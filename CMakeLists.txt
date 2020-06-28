cmake_minimum_required(VERSION 3.16)
project(cgl)

set(CMAKE_CXX_STANDARD 17)

add_subdirectory(glad)

add_library(cgl INTERFACE)
target_include_directories(cgl INTERFACE include)
add_dependencies(cgl PUBLIC glad)
