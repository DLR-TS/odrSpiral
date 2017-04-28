cmake_minimum_required(VERSION 2.6)

project (odrSpiral)

# SHARED library output directory
#set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}/bin)
# STATIC library output directory
set(CMAKE_ARCHIVE_OUTPUT_DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}/lib)

include_directories(${CMAKE_CURRENT_SOURCE_DIR}/include)
#add_library(odrSpiral SHARED src/odrSpiral.c)
add_library(libOdrSpiral STATIC src/odrSpiral.c)

