# Main cmakelists.txt
# @author : Ziad Mostafa

cmake_minimum_required(VERSION 3.9.2)

set(PROJECT_DESCRIPTION "\"A group project for Course 1 of C++ Nano Degree \
     assignments and development\"")

# Include common project macros
set(CMAKE_MODULE_PATH ${CMAKE_MODULE_PATH} ${CMAKE_CURRENT_SOURCE_DIR}/../../cmake)

# C++ Executable 
add_executable('week-one')
