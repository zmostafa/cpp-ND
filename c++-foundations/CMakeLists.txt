# Main cmakelists.txt
# @author : Ziad Mostafa

cmake_minimum_required(VERSION 3.9.2)

set(PROJECT_DESCRIPTION "\"A group project for Course 1 of C++ Nano Degree \
     assignments and development\"")

# Include common project macros
set(CMAKE_MODULE_PATH ${CMAKE_MODULE_PATH} ${CMAKE_CURRENT_SOURCE_DIR}/../cmake)

# Set the version number of your project here (format is MAJOR.MINOR.PATCHLEVEL - e.g. 1.0.0)
set(VERSION_MAJOR "0")
set(VERSION_MINOR "0")
set(VERSION_PATCH "0")
set(VERSION ${VERSION_MAJOR}.${VERSION_MINOR}.${VERSION_PATCH})

# Add directory c++-Foundations that contains the work of the first part of the ND
add_subdirectory('week-one')
