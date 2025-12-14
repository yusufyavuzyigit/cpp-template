cmake_minimum_required(VERSION 3.60)
project(ProjName LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

include(Cmake/CPM.cmake)

add_subdirectory(App)
add_subdirectory(Core)

# May work, may not work. If works, nice.
if(MSVC)
    set_property(GLOBAL PROPERTY VS_STARTUP_PROJECT App)
endif()