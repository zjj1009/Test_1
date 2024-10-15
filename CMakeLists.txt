cmake_minimum_required(VERSION 3.28.0)

project(HelloWorld)

add_library(a
    src/a.cpp
)

add_executable(main
    src/main.cpp
)

target_link_libraries(main a)
target_include_directories(main PRIVATE include)