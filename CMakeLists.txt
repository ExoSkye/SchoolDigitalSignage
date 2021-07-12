cmake_minimum_required(VERSION 3.15)

cmake_policy(SET CMP0091 NEW)
enable_language(CXX)

project(SchoolDigitalSignage)

set(CMAKE_CXX_STANDARD 20)

add_executable(CI_TEST test.cpp)
set_property(TARGET CI_TEST PROPERTY MSVC_RUNTIME_LIBRARY "MultiThreaded")
