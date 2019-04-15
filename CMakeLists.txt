# Main cmakelists.txt
# @author : Ziad Mostafa

cmake_minimum_required(VERSION 3.10.2)

project('CPP-ND')
set(PROJECT_DESCRIPTION "\"A group project for all assignments and development \
                        in Udacity C++ Nano Degree\"")

# Include common project macros
set(CMAKE_MODULE_PATH ${CMAKE_MODULE_PATH} ${CMAKE_CURRENT_SOURCE_DIR}/cmake)

set(CMAKE_CXX_STANDARD 14) # Set C++14 as langugae standard.
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -Wall -Wextra -Werror -O2 -g")

enable_testing() # needed on top-level CMakeLists.txt
add_custom_target(doc)

# Add directory c++-Foundations that contains the work of the first part of the ND
add_subdirectory('c++-foundations')
