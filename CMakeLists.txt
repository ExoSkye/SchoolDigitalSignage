cmake_minimum_required(VERSION 3.10)

project(SchoolDigitalSignage)

set(CMAKE_CXX_STANDARD 20)
set_property(GLOBAL PROPERTY MSVC_RUNTIME_LIBRARY "MultiThreaded$<$<CONFIG:Debug>:Debug>")

add_executable(CI_TEST test.cpp)
