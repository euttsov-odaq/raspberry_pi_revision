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
add_library(tablelib
    table.c
    raspberry_pi_revision.c
    raspberry_pi_revision.h
)
set_target_properties(tablelib PROPERTIES
    OUTPUT_NAME table
)
