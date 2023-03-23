cmake_minimum_required(VERSION 3.23)

project(solver)

set(CMAKE_CXX_STANDARD 14)

include_directories(${CMAKE_CURRENT_SOURCE_DIR}/formatter_ex_lib)

add_subdirectory(${CMAKE_CURRENT_SOURCE_DIR}/formatter_ex_lib)

include_directories(${CMAKE_CURRENT_SOURCE_DIR}/solver_lib)

add_subdirectory(${CMAKE_CURRENT_SOURCE_DIR}/solver_lib)

add_executable(solver ${CMAKE_CURRENT_SOURCE_DIR}/solver_application/equation.cpp)

target_link_libraries(solver formatter_ex solver_lib)
