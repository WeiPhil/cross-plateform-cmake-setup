cmake_minimum_required(VERSION 3.1)

# Project name
project(SFMLTest)

add_subdirectory(ext ext_build)

include_directories(
  # Project include files
  #${CMAKE_CURRENT_SOURCE_DIR}/include

  # SFML
  ${SFML_INCLUDE_DIRS}

  # GLEW
  ${GLEW_INCLUDE_DIRS}
)

add_executable(SFMLTest

  # Source files
  src/main.cpp

)

# Linking libraries to project
target_link_libraries(SFMLTest sfml-graphics sfml-audio glew)