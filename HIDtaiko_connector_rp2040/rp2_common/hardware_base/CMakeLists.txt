add_library(hardware_base INTERFACE)
add_library(hardware_base_headers INTERFACE)
target_include_directories(hardware_base_headers SYSTEM INTERFACE ${CMAKE_CURRENT_LIST_DIR}/include)
target_link_libraries(hardware_base_headers INTERFACE pico_base_headers)
target_link_libraries(hardware_base INTERFACE hardware_base_headers)