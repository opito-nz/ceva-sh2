zephyr_library()

zephyr_include_directories(${CMAKE_CURRENT_SOURCE_DIR})

zephyr_library_sources_ifdef(CONFIG_CEVA_SH2 euler.c)
zephyr_library_sources_ifdef(CONFIG_CEVA_SH2 sh2.c)
zephyr_library_sources_ifdef(CONFIG_CEVA_SH2 sh2_SensorValue.c)
zephyr_library_sources_ifdef(CONFIG_CEVA_SH2 sh2_util.c)
zephyr_library_sources_ifdef(CONFIG_CEVA_SH2 shtp.c)
