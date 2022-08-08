cmake_minimum_required(VERSION 3.18)
project(example1 VERSION 1.0)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED True)

add_executable(example1
        tutorial.cxx)

configure_file(config.h.in config.h)

target_include_directories(example1 PUBLIC
        "${PROJECT_BINARY_DIR}"
        )


