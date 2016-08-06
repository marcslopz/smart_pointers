cmake_minimum_required(VERSION 2.6)
project(smart_pointers)

set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -pthread")
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -pthread")
set(CMAKE_EXE_LINKER_FLAGS "${CMAKE_EXE_LINKER_FLAGS} -pthread")

add_executable(
  smart_pointers
  src/main.cpp
  )
target_compile_features(smart_pointers PRIVATE cxx_range_for)
