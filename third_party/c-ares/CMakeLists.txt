set(CARES_STATIC ON)
set(CARES_SHARED OFF)
set(CARES_INSTALL OFF)
set(CARES_STATIC_PIC ON)
set(CARES_BUILD_TESTS OFF)
set(CARES_BUILD_TOOLS OFF)

string(REPLACE "-Wconversion" "" CMAKE_C_FLAGS "${CMAKE_C_FLAGS}")
string(REPLACE "-Wconversion" "" CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS}")

add_subdirectory(repo)

target_include_directories(c-ares
    PUBLIC
    
    $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}/repo>
    $<INSTALL_INTERFACE:repo>
)