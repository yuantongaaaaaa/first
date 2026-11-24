cmake_minimum_required(VERSION 4.3)
project(first C)

set(CMAKE_C_STANDARD 11)

add_executable(first main.c test1.h
        20141101C1/b.c)
target_link_libraries(first test1)

add_executable(test test.c test1.h)
target_link_libraries(test test1)

add_library(test1 test1.c test1.h)
