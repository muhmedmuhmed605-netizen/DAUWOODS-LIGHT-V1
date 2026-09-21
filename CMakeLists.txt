cmake_minimum_required(VERSION 3.10.2)
project("DAUWOODS-LIGHT")

add_library(
    dauwood-light
    SHARED
    DAUWOOD'S LIGHT.cxx
)

find_library(
    log-lib
    log
)

target_link_libraries(
    dauwood-light
    ${log-lib}
)
