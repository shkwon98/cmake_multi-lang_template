cmake_minimum_required(VERSION 3.12)
project(HelloWorld)

set(CMAKE_BUILD_TYPE Debug)
set(CMAKE_EXPORT_COMPILE_COMMANDS ON)
set(CMAKE_VERBOSE_MAKEFILE ON CACHE BOOL "Makefile Verbose")
set(CMAKE_INSTALL_PREFIX ${CMAKE_SOURCE_DIR}/bin)

add_subdirectory(C)
add_subdirectory(C++)
add_subdirectory(Go)