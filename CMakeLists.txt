cmake_minimum_required(VERSION 3.5)

project(assignment6_5__1_QC_CORR LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_subdirectory(/home/max/libpqxx-7.8.1 pqxx-build)
add_executable(assignment6_5__1_QC_CORR main.cpp
    table_class.cpp
    table_class.h)

target_link_libraries(assignment6_5__1_QC_CORR PRIVATE pqxx)
