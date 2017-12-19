cmake_minimum_required (VERSION 2.8.3)
project (PCA9685)
add_library(PCA9685 SHARED
    PCA9685.cpp
    I2C.cpp
)

install(
    TARGETS PCA9685
    DESTINATION ${CMAKE_INSTALL_PREFIX}
)

install(
    FILES I2C.h PCA9685.h
    DESTINATION ${CMAKE_INSTALL_PREFIX}/include/
)

