# Main cmakelists.txt
# @author : Ziad Mostafa

cmake_minimum_required(VERSION 3.5.1)

set(PROJECT_DESCRIPTION "\"A group project for Course 1 of C++ Nano Degree \
     assignments and development\"")

# Include common project macros
set(CMAKE_MODULE_PATH ${CMAKE_MODULE_PATH} ${CMAKE_CURRENT_SOURCE_DIR}/../../cmake)

# C++ Executable 
add_executable(PrintBoard main.cpp)

add_custom_target(copy-maze-file)
add_custom_command(
        TARGET foo POST_BUILD
        COMMAND ${CMAKE_COMMAND} -E copy
                ${CMAKE_SOURCE_DIR}/maze.board
                ${CMAKE_CURRENT_BINARY_DIR}/maze.baord)