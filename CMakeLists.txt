cmake_minimum_required(VERSION 3.14...3.20)

project(
  ScopeGuard
  LANGUAGES CXX)

if(CMAKE_PROJECT_NAME STREQUAL PROJECT_NAME)
  set(CMAKE_CXX_STANDARD 17)
  set(CMAKE_CXX_EXTENSIONS OFF)

  set_property(GLOBAL PROPERTY USE_FOLDERS ON)
endif()

add_library(scopeguard INTERFACE)
target_include_directories(scopeguard INTERFACE include/)
