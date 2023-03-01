cmake_minimum_required(VERSION 3.20)

# set the project name
project(CollisionMap)

# specify the C++ standard
set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED True)

add_library(CollisionMap)
add_executable(CollisionMap)

target_include_directories(CollisionMap PRIVATE
    include
    src
)

target_link_libraries(CollisionMap)

add_subdirectory(src)