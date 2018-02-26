cmake_minimum_required(VERSION 2.8 FATAL_ERROR)

project(qt_editable_tree_view)

SET(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=gnu++11")

find_package(Qt4 REQUIRED)
INCLUDE         (${QT_USE_FILE})
ADD_DEFINITIONS (${QT_DEFINITIONS})


set(CMAKE_INCLUDE_CURRENT_DIR ON)
include_directories(${CMAKE_SOURCE_DIR}/src)
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_SOURCE_DIR}/bin)
set(CMAKE_LIBRARY_OUTPUT_DIRECTORY ${CMAKE_SOURCE_DIR}/lib)
set(CMAKE_SHARED_LIBRARY_SUFFIX .so)

# Add code
include_directories("${PROJECT_BINARY_DIR}")
add_subdirectory(src)
