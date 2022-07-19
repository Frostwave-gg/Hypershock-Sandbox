cmake_minimum_required(VERSION 3.20.0)

project(Hypershock-Game VERSION 0.0.1)

set(CMAKE_RUNTIME_OUTPUT_DIRECTORY "${CMAKE_CURRENT_SOURCE_DIR}/bin/Sandbox")

add_executable(Hypershock-Game "${CMAKE_CURRENT_SOURCE_DIR}/Sandbox/src/main.cpp")

add_subdirectory("${CMAKE_CURRENT_SOURCE_DIR}/Sandbox/Engine/Hypershock")

target_link_libraries(Hypershock-Game PRIVATE Hypershock)