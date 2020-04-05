# Set the minimum version of CMake that can be used
# To find the cmake version run
# $ cmake --version
cmake_minimum_required(VERSION 3.5)

# Set the project name
project (fe)
#_CRT_SECURE_NO_WARNINGS
# Add an executable


add_executable(fe ./src/fe.c ./src/fe.h)

if(WIN32)
    target_compile_definitions(fe PUBLIC _CRT_SECURE_NO_WARNINGS)
endif()