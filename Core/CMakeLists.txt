add_library(Core)

target_sources(Core
    PRIVATE
        src/core.cpp
)

target_include_directories(Core
    PUBLIC
        ${CMAKE_CURRENT_SOURCE_DIR}/include
    PRIVATE
        ${CMAKE_CURRENT_SOURCE_DIR}/src
)

target_compile_features(Core PUBLIC cxx_std_17)
