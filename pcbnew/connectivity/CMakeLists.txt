include_directories( BEFORE ${INC_BEFORE} )

include_directories(
    ./
    ../
    ../../include
    ../../polygon
    ${INC_AFTER}
)

set( PCBNEW_CONN_SRCS
    connectivity_algo.cpp
    connectivity_data.cpp
    connectivity_items.cpp
)

add_library( connectivity STATIC ${PCBNEW_CONN_SRCS} )
