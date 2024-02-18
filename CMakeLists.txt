cmake_minimum_required(VERSION 3.27)

project(cppstarter)

# Main vars.
set(SRC_DIR ${CMAKE_SOURCE_DIR}/src)

# Sources.
add_executable(${CMAKE_PROJECT_NAME}
    ${SRC_DIR}/main.cpp
    ${SRC_DIR}/main.h
)

# Libs.

# Standarts.
set_property(TARGET ${CMAKE_PROJECT_NAME} PROPERTY CXX_STANDARD 23)
set_property(TARGET ${CMAKE_PROJECT_NAME} PROPERTY CXX_STANDARD_REQUIRED ON)
set_property(TARGET ${CMAKE_PROJECT_NAME} PROPERTY CXX_EXTENSIONS OFF)

# Link.