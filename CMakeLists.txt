cmake_minimum_required(VERSION 3.15)

cmake_policy(SET CMP0091 NEW)
enable_language(CXX)

project(SchoolDigitalSignage)

set(CMAKE_CXX_STANDARD 20)

option(BUILD_SERVICE "Build the *Windows* Service - this won't build on anything other than Windows" ON)
option(BUILD_CLIENT "Build the Linux Client - requires SDL2 to be installed" ON)

if (BUILD_SERVICE)
	add_subdirectory(SDSService)
endif()

if (BUILD_CLIENT)
	add_subdirectory(SDSClient)
endif()
