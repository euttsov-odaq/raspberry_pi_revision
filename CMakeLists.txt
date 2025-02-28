cmake_minimum_required(VERSION 3.30)
project(rpi_revision)
add_executable(test
    test.c
    raspberry_pi_revision.c
    raspberry_pi_revision.h
)
add_executable(table
    table.c
    raspberry_pi_revision.c
    raspberry_pi_revision.h
)
add_library(rpi_revision
    table.c
    raspberry_pi_revision.c
    raspberry_pi_revision.h
)
target_include_directories(rpi_revision
    PUBLIC ${CMAKE_CURRENT_LIST_DIR} ${CMAKE_CURRENT_BINARY_DIR}
)
