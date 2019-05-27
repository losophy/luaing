cmake_minimum_required(VERSION 2.8)

project(regEngine)
add_definitions(-std=c++11)

aux_source_directory(. DIR_SRCS)

add_executable(regEngine ${DIR_SRCS})
