cmake_minimum_required(VERSION 3.23)

project(formatter_ex)

add_subdirectory(../formatter_lib formatter)

include_directories(../formatter_lib formatter)


add_library(formatter_ex STATIC formatter_ex.cpp formatter_ex.h)

target_link_libraries(formatter_ex formatter)
