cmake_minimum_required(VERSION 3.10)
project(NrfLibGeneral VERSION 1.0.0)

zephyr_library_named(NrfLibGeneral)

zephyr_library_include_directories(include)
target_include_directories(NrfLibGeneral INTERFACE $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}/include>)
zephyr_library_sources(src/led.cpp)
