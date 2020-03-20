include_directories(${CMAKE_SOURCE_DIR}/include )

set(SOURCES  main.cpp)

add_executable( picking_colorbuffer ${SOURCES} )
target_link_libraries(picking_colorbuffer opengl32  ${COMMON_LIBRARY} ${GLEW_LIBRARY} ${GLFW3_LIBRARY})
