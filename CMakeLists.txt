cmake_minimum_required(VERSION 3.5)

project(bb_blue_api)

add_subdirectory(libraries)

add_executable(gyro_test examples/calibrate_gyro/calibrate_gyro.c)

target_link_libraries(gyro_test bb_blue)