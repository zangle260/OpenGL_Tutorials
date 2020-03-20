include_directories(${CMAKE_SOURCE_DIR}/include )

set(SOURCES  main.cpp)

add_executable( hello_window ${SOURCES} )
target_link_libraries(hello_window opengl32  ${COMMON_LIBRARY} ${GLEW_LIBRARY} ${GLFW3_LIBRARY})
