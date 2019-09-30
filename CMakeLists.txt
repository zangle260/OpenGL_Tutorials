cmake_minimum_required (VERSION 2.8)

project (GLToturials)

list(APPEND CMAKE_CXX_FLAGS "-std=c++11")

set(EXECUTABLE_OUTPUT_PATH  "${CMAKE_SOURCE_DIR}/bin")
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_SOURCE_DIR}/bin)
set(CMAKE_MODULE_PATH ${CMAKE_MODULE_PATH} "${CMAKE_SOURCE_DIR}/cmake")

find_package(GLEW REQUIRED)
if(NOT GLEW_FOUND)
   message(ERROR "-- GLEW not found!")
endif(NOT GLEW_FOUND)
    
find_package(GLFW3 REQUIRED)
if(NOT GLFW3_FOUND)
   message(ERROR "-- GLFW3 not found!")
endif(NOT GLFW3_FOUND)


add_subdirectory(src/common)
add_subdirectory(src/hello_window)
#add_subdirectory( ingredients )
#add_subdirectory( chapter01 )
#add_subdirectory( chapter02 )
#add_subdirectory( chapter03 )
#add_subdirectory( chapter04 )
#add_subdirectory( chapter05 )
#add_subdirectory( chapter06 )
#add_subdirectory( chapter07 )
#add_subdirectory( chapter08 )
#add_subdirectory( chapter09 )

