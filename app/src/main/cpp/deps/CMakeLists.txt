cmake_minimum_required(VERSION 3.12)
project(deps)

set(GLAD_SOURCES_DIR "${PROJECT_SOURCE_DIR}/glad")
add_subdirectory("${GLAD_SOURCES_DIR}/cmake" glad_cmake)
glad_add_library(glad REPRODUCIBLE MX API gles2:core=3.0)
