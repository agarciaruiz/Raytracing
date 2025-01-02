cmake_minimum_required ( VERSION 3.1.0...3.27.0 )

project(Raytracing LANGUAGES CXX)

set ( CMAKE_CXX_STANDARD          17 )
set ( CMAKE_CXX_STANDARD_REQUIRED ON )
set ( CMAKE_CXX_EXTENSIONS        OFF )

set ( SOURCE
  src/main.cpp
)

include_directories(src)

add_executable(Raytracing ${SOURCE})