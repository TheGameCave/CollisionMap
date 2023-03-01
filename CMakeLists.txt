cmake_minimum_required(VERSION 3.20)

# set the project name
project(CollisionMap)

# specify the C++ standard
set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED True)

add_library(CollisionMap)

target_include_directories(CollisionMap PUBLIC
    include
    src
)

target_link_libraries(CollisionMap)

add_subdirectory(src)

if(CMAKE_CURRENT_SOURCE_DIR STREQUAL CMAKE_SOURCE_DIR)
    message(STATUS "GOT HERE!")
endif()