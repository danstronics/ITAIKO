pico_simple_hardware_target(adc)

# additional library
pico_mirrored_target_link_libraries(hardware_adc INTERFACE hardware_gpio hardware_resets)