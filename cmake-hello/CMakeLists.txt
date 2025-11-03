cmake_minimum_required(VERSION 3.20)

# https://cmake.org/cmake/help/v4.1/command/project.html
project(Hello LANGUAGES NONE)
message("configure-time message from CMake")

add_custom_target(
  greet
  COMMAND echo "build-time message from CMake"
)
