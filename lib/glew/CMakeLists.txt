cmake_minimum_required (VERSION 2.6)
project (glew)

set (GLEW_INCLUDE_DIRS "${PROJECT_SOURCE_DIR}/include" CACHE INTERNAL "")
set (GLEW_SRC_DIR      "${PROJECT_SOURCE_DIR}/src" CACHE INTERNAL "")

file(GLOB_RECURSE SOURCES "${GLEW_SRC_DIR}/*.c")

include_directories("${GLEW_INCLUDE_DIRS}")

add_library(glew STATIC ${SOURCES})
target_compile_definitions(glew PUBLIC -DGLEW_STATIC)
