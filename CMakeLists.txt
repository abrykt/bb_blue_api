cmake_minimum_required(VERSION 3.5)

project(bb_blue_api)
include_directories(libraries)
add_subdirectory(libraries)

macro(add_exe NAME)
    add_executable(${NAME} examples/${NAME}/${NAME}.c)
    target_link_libraries(${NAME} bb_blue pthread m)
endmacro()

add_exe(calibrate_gyro)
add_exe(test_imu)

