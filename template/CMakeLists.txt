cmake_minimum_required(VERSION 3.24)

set(CURRENT_PROJECT_NAME template)

file(GLOB src_files src/*.cpp)
set(TEST_NAME test_${CURRENT_PROJECT_NAME})

project(${CURRENT_PROJECT_NAME} VERSION 1 LANGUAGES CXX)
set(CMAKE_CXX_STANDARD 20)

add_executable(${CURRENT_PROJECT_NAME} ${src_files})
target_include_directories(${CURRENT_PROJECT_NAME} PUBLIC inc)

add_executable(${TEST_NAME} ${src_files})
target_include_directories(${TEST_NAME} PUBLIC inc)
target_compile_definitions(${TEST_NAME} PUBLIC TESTING=${CURRENT_PROJECT_NAME})
add_test(NAME ${TEST_NAME} COMMAND ${TEST_NAME})
