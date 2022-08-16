cmake_minimum_required(VERSION 3.20)

include(./cmake/CompilerWarnings.cmake)
include(./cmake/option.cmake)

project(SDL2_CPP LANGUAGES CPP)

set (SRCS
    src/main.cpp
)

set (HEADERS
)

add_library(SDL2_CPP STATIC ${SRCS} ${HEADERS})
SET_TARGET_WARNINGS(SDL2_CPP)