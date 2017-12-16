cmake_minimum_required (VERSION 2.8.3)
project (PCA9685)
add_library(PCA9685 SHARED
    PCA9685.cpp
    I2C.cpp
)
