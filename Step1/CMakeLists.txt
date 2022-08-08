cmake_minimum_required(VERSION 3.18)
project(Tutorial1 VERSION 1.0)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED True)

add_executable(Tutorial1
        tutorial.cxx)

configure_file(config.h.in config.h)

target_include_directories(Tutorial1 PUBLIC
        "${PROJECT_BINARY_DIR}"
        )


