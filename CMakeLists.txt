cmake_minimum_required(VERSION 3.1 FATAL_ERROR)

project(cpp_template)

set(EXECUTABLE_NAME a.out)

include_directories("src")

set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ../bin)

# Shared library directory
set(CMAKE_LIBRARY_OUTPUT_DIRECTORY ../lib)

# Static library directory
set(CMAKE_ARCHIVE_OUTPUT_DIRECTORY ../lib)

set(CMAKE_CXX_FLAGS "-g -Wall")

add_executable(${EXECUTABLE_NAME} src/main.cpp)