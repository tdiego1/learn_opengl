project(glfw3)

add_library(glfw3 STATIC IMPORTED GLOBAL)
set_target_properties(glfw3 PROPERTIES LINKER_LANGUAGE C)
set_target_properties(glfw3 PROPERTIES IMPORTED_LOCATION ${PROJECT_SOURCE_DIR}/bin/libglfw3.a)

target_include_directories(glfw3 INTERFACE ${PROJECT_SOURCE_DIR}/inc)


