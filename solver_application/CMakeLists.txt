cmake_minimum_required(VERSION 3.22.1 FATAL_ERROR)
project(solver)
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
<<<<<<< HEAD
add_subdirectory(${CMAKE_CURRENT_SOURCE_DIR}/../formatter_ex_lib formtr_ex)
add_subdirectory(${CMAKE_CURRENT_SOURCE_DIR}/../solver_lib slver)
add_executable(solver ${CMAKE_CURRENT_SOURCE_DIR}/equation.cpp)
target_link_libraries(solver formatter_ex_lib solver_lib)
=======
add_subdirectory(${CMAKE_CURRENT_SOURCE_DIR}/../formatter_ex_lib frmtr_ex)
add_subdirectory(${CMAKE_CURRENT_SOURCE_DIR}/../solver_lib slvr)
add_executable(solver ${CMAKE_CURRENT_SOURCE_DIR}/src/equation.cpp)
target_include_directories(formatter_ex_lib PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/../formatter_ex_lib/src ${CMAKE_CURRENT_SOURCE_DIR}/../solver_lib/src)
target_link_libraries(solver formatter_ex_lib solver_lib)

>>>>>>> d36061e (update v2)
