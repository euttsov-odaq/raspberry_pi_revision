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

