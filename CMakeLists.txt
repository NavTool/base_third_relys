#libevent option
# set(EVENT_LIBRARY_TYPE STATIC)
# set(EVENT__LIBRARY_TYPE STATIC)
set(EVENT__DISABLE_OPENSSL ON)
set(EVENT__DISABLE_BENCHMARK ON)
set(EVENT__DISABLE_TESTS ON)
set(EVENT__DISABLE_REGRESS ON)
set(EVENT__DISABLE_SAMPLES ON)
add_subdirectory(libevent)

#hiredis option
set(BUILD_SHARED_LIBS OFF)
set(DISABLE_TESTS ON)
add_subdirectory(hiredis)

#yaml-cpp option
set(YAML_BUILD_SHARED_LIBS OFF)
set(YAML_CPP_BUILD_TOOLS OFF)
add_subdirectory(yaml-cpp)

# add_subdirectory(libssh2-libssh2-1.11.0/)

# #json
# set(JSON_INCLUDE_PATH "${CMAKE_CURRENT_SOURCE_DIR}/json/include")

# #spdlog
# set(SPDLOG_INCLUDE_PATH "${CMAKE_CURRENT_SOURCE_DIR}/spdlog/include")