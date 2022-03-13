cmake_minimum_required(VERSION 3.21)
project(cmake_test C)

set(CMAKE_C_STANDARD 23)

file(GLOB SRC
        src/*.c
        main.c
        )

add_executable(cmake_test ${SRC})

target_include_directories(cmake_test
        PRIVATE
        include/*.h
        )