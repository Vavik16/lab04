cmake_minimum_required(VERSION 3.23)
project(hello_world_application)

set(CMAKE_CXX_STANDARD 14)

include_directories(${CMAKE_CURRENT_SOURCE_DIR}/formatter_ex_lib)

add_subdirectory(formatter_ex_lib)

add_executable(hello_world_application hello_world.cpp)

target_link_libraries(hello_world_application formatter_ex)
