if(CONFIG_LIB_GPS_SAM_M10Q)
zephyr_interface_library_named(LIB_GPS_SAM_M10Q)

zephyr_include_directories(.)

zephyr_library()
zephyr_library_sources(
    sam_m10q/src/sample.c
)

zephyr_library_link_libraries(LIB_GPS_SAM_M10Q)
target_link_libraries(LIB_GPS_SAM_M10Q INTERFACE zephyr_interface)
endif()