cmake_minimum_required(VERSION 2.8)

project(regEngine)
add_definitions(-std=c++11)

aux_source_directory(. DIR_SRCS)
SET(EXECUTABLE_OUTPUT_PATH ${PROJECT_BINARY_DIR}/../bin)  

SET(CMAKE_BUILD_TYPE "Debug")
SET(CMAKE_CXX_FLAGS_DEBUG "$ENV{CXXFLAGS} -O0 -Wall -g2 -ggdb")
SET(CMAKE_CXX_FLAGS_RELEASE "$ENV{CXXFLAGS} -O3 -Wall")

add_executable(regEngine ${DIR_SRCS})
