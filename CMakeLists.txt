cmake_minimum_required(VERSION 2.8)

# Make PROJECT_SOURCE_DIR, PROJECT_BINARY_DIR, and PROJECT_NAME available.
set(PROJECT_NAME TestProject)
project(${PROJECT_NAME})

set(CMAKE_CXX_FLAGS "-g -Wall")


add_executable(project1 main.cpp)

# Testing
if (APPLE)
add_definitions(-DGTEST_USE_OWN_TR1_TUPLE)
add_definitions(-D__GLIBCXX__)
endif (APPLE)

add_subdirectory(lib/gtest)
enable_testing()
include_directories(${gtest_SOURCE_DIR}/include ${gtest_SOURCE_DIR})

# Unit Tests
add_executable(runUnitTests test.cpp)

target_link_libraries(runUnitTests gtest gtest_main)

# This is so you can do 'make test' to see all your tests run, instead of
# manually running the executable runUnitTests to see those specific tests.
add_test(NAME test COMMAND runUnitTests)
