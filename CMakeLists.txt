cmake_minimum_required ( VERSION 3.1.0...3.27.0 )

project(Raytracing LANGUAGES CXX)

set ( CMAKE_CXX_STANDARD          17 )
set ( CMAKE_CXX_STANDARD_REQUIRED ON )
set ( CMAKE_CXX_EXTENSIONS        OFF )

set(SRC_DIR ${CMAKE_SOURCE_DIR}/src)

set ( SOURCE
    ${SRC_DIR}/main.cpp
    ${SRC_DIR}/ray.h
    ${SRC_DIR}/color.h
    ${SRC_DIR}/vec3.h
    ${SRC_DIR}/hittable.h
    ${SRC_DIR}/hittable_list.h
    ${SRC_DIR}/sphere.h
    ${SRC_DIR}/rtweekend.h
    ${SRC_DIR}/interval.h
)

source_group("Source Files" FILES ${SRC_DIR}/main.cpp)
source_group("Header Files" FILES ${SRC_DIR}/ray.h ${SRC_DIR}/color.h ${SRC_DIR}/vec3.h)

include_directories(${SRC_DIR})

add_executable(Raytracing ${SOURCE})