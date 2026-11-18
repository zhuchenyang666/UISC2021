cmake_minimum_required(VERSION 3.16)

project(UICS2021 LANGUAGES CXX)

add_executable(UICS2021 main.cpp)
set_target_properties(UICS2021 PROPERTIES
    CXX_STANDARD 17
    CXX_STANDARD_REQUIRED YES
    CXX_EXTENSIONS NO
)
