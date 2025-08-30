cmake_minimum_required(VERSION 3.20)
project(srjcore C)

set(CMAKE_C_STANDARD 99)

add_library(srjcore STATIC
    src/srjcore.c
)
target_include_directories(srjcore PUBLIC include)

install(TARGETS srjcore DESTINATION lib)
install(DIRECTORY include/ DESTINATION include)
