include_directories(${CMAKE_SOURCE_DIR}/include )

file(GLOB SOURCES ${CMAKE_CURRENT_SOURCE_DIR}/*.cpp)

add_library(common_library STATIC ${SOURCES} )

