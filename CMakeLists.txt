cmake_minimum_required(VERSION 3.1)

# Project name
project(YOUR_PROJECT_NAME)

add_subdirectory(ext ext_build)

include_directories(
  # Project include files
  #${CMAKE_CURRENT_SOURCE_DIR}/include

  # SFML
  ${SFML_INCLUDE_DIRS}

  # GLEW
  ${GLEW_INCLUDE_DIRS}
)

add_executable(YOUR_PROJECT_NAME

  # Source files
  src/main.cpp

)

# Linking libraries to project
target_link_libraries(YOUR_PROJECT_NAME sfml-graphics sfml-audio glew)