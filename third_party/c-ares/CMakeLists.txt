set(CARES_SHARED OFF)
set(CARES_STATIC ON)
set(CARES_STATIC_PIC ON)
set(CARES_BUILD_TESTS OFF)
set(CARES_BUILD_TOOLS OFF)

add_subdirectory(repo)

target_include_directories(ot-config INTERFACE ${CMAKE_CURRENT_SOURCE_DIR}/repo/include)

target_link_libraries(ot-config INTERFACE c-ares::cares)