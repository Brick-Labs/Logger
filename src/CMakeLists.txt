add_library(${PROJECT_NAME} STATIC
        Logger.cpp
)

# Namespace-Alias
add_library(Logger::Logger ALIAS Logger)

# Add Include-Path
target_include_directories(Logger
        PUBLIC
        $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}/../include>
        PRIVATE
        ${CMAKE_CURRENT_SOURCE_DIR}
)
