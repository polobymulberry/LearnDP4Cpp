cmake_minimum_required(VERSION 3.12)

if(CMAKE_SOURCE_DIR STREQUAL CMAKE_BINARY_DIR)
    message(FATAL_ERROR "Do not build in-source. Please remove CMakeCache.txt and the CMakeFiles/ directory. Then build out-of-source.")
endif()

project(SimpleFactoryPattern)

set(SFP_SOURCE_FILES main.cpp)

add_executable(SimpleFactoryPattern ${SFP_SOURCE_FILES})