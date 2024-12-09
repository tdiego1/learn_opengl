project(basic_opengl)

set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${PROJECT_SOURCE_DIR}/bin)
set(CMAKE_LIBRARY_OUTPUT_DIRECTORY ${PROJECT_SOURCE_DIR}/bin)

set(BASIC_OPENGL_INCLUDES ${PROJECT_SOURCE_DIR}/inc/basic_opengl/basic_opengl_main.h)

set(BASIC_OPENGL_SOURCES ${PROJECT_SOURCE_DIR}/src/basic_opengl_main.c)

add_executable(basic_opengl ${BASIC_OPENGL_SOURCES} ${BASIC_OPENGL_INCLUDES})

target_link_libraries(basic_opengl PRIVATE glfw3 glad)

