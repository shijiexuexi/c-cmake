file(GLOB source "*.cpp")

add_library(src ${source})

target_include_directories(src PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})

set(EXECUTABLE_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/bin)