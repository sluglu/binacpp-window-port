cmake_minimum_required(VERSION 3.5)
project(binacpp)

# Set C++ standard
set(CMAKE_CXX_STANDARD 14)

file(GLOB SOURCE_FILES ${CMAKE_CURRENT_SOURCE_DIR}
	*.cpp
	*.c
	*.h
	*.hpp)

add_library(${PROJECT_NAME} ${SOURCE_FILES})

target_include_directories(${PROJECT_NAME} PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})

