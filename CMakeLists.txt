cmake_minimum_required(
    VERSION 3.13
)

project(talented_hack LANGUAGES C CXX)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

set(LV2_INCLUDE_DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}/libs/lv2)
include(cmake/lv2.cmake)

option(USER_DYN_MANIFEST "Dynmanifest plugin" OFF)
option(ENABLE_PROFILER "Enable the profiler library" OFF)

include_directories(./include ./src)

