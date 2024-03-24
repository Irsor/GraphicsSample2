cmake_minimum_required(VERSION 3.21.3)

# Название проекта
set(PROJECT_NAME GraphicsSample2)
project(${PROJECT_NAME} VERSION 0.1.0 LANGUAGES C CXX)

# Исходный код
set(SOURCES
    src/main.cpp
)

# GLFW
set(GLFW_BUILD_DOCS OFF CACHE BOOL "" FORCE)
set(GLFW_INSTALL OFF CACHE BOOL "" FORCE)
set(GLFW_BUILD_TESTS OFF CACHE BOOL "" FORCE)
set(GLFW_BUILD_EXAMPLES OFF CACHE BOOL "" FORCE)
set(GLFW_USE_HYBRID_HPG ON CACHE BOOL "" FORCE)

# Подмодули
add_subdirectory(external/glad)

add_executable(${PROJECT_NAME} ${SOURCES})
target_link_libraries(${PROJECT_NAME} glad)
