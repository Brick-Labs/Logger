add_subdirectory(spdlog)

target_link_libraries(Logger PRIVATE spdlog::spdlog)
