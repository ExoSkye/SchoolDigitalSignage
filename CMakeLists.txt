cmake_minimum_required(VERSION 3.10)

project(SchoolDigitalSignage)

set(CMAKE_CXX_STANDARD 20)

add_executable(CI_TEST test.cpp)
set_property(TARGET CI_TEST PROPERTY MSVC_RUNTIME_LIBRARY "MultiThreaded$<$<CONFIG:Debug>:Debug>")
