cmake_minimum_required(VERSION 3.7)
project(Filters)

include(filters.cmake)

add_definitions(-fpic)

SET(AVIF_SRC
        ${CMAKE_CURRENT_SOURCE_DIR}/dmx_avif.c
)

SET(AVIF_INC
        ${CMAKE_CURRENT_SOURCE_DIR}/include
)

add_filter(avif
        "${AVIF_SRC}"
        ""
        []
        ""
        "${AVIF_INC}"
        ""
        "1")
