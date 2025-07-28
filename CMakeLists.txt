cmake_minimum_required(VERSION 3.10)
project(NrfLibGeneral VERSION 1.0.0)

add_library(NrfLibGeneral INTERFACE)

target_include_directories(NrfLibGeneral INTERFACE $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}/include>)


