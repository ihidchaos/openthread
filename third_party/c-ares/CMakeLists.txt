set(CARES_SHARED OFF)
set(CARES_STATIC ON)

add_subdirectory(repo)

target_include_directories(c-ares
    PUBLIC
    
    $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}/repo>
    $<INSTALL_INTERFACE:repo>
)