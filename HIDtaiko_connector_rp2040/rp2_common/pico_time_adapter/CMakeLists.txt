pico_add_library(pico_time_adapter)

target_include_directories(pico_time_adapter_headers SYSTEM INTERFACE ${CMAKE_CURRENT_LIST_DIR}/include)

pico_mirrored_target_link_libraries(pico_time INTERFACE pico_time_adapter)