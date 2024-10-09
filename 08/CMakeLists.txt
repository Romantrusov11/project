cmake_minimum_required(VERSION 3.20)

set(TARGET "vec")

set(HEADERS
    ${LIB_DIR}/vec/vec2d.h
)
set(SOURCES
    main.cpp
    ${LIB_DIR}/vec/vec2d.cpp
)

project(${TARGET} CXX)

add_executable(${TARGET} ${HEADERS} ${SOURCES})
cmake_path(SET LIB_DIR ${LIB_DIR})

install(TARGETS ${TARGET})