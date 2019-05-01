# Main cmakelists.txt
# @author : Ziad Mostafa

cmake_minimum_required(VERSION 3.9.2)

set(PROJECT_DESCRIPTION "\"A group project for Course 1 of C++ Nano Degree \
     assignments and development\"")

# Include common project macros
set(CMAKE_MODULE_PATH ${CMAKE_MODULE_PATH} ${CMAKE_CURRENT_SOURCE_DIR}/../../cmake)


include_directories(
    ${PROJECT_SOURCE_DIR}/include
    ${PROJECT_BINARY_DIR}/include   # add the binary tree to the search path so that we will find Version.h
)

# Add directory c++-Foundations that contains the work of the first part of the ND
enable_testing()
add_subdirectory(include)
add_subdirectory(src)
add_subdirectory(doc)
add_subdirectory(test)

