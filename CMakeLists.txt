cmake_minimum_required(VERSION 3.20.0)

project(Hypershock-Game VERSION 0.0.1)

add_executable(Hypershock-Game "${CMAKE_CURRENT_SOURCE_DIR}/Sandbox/src/main.cpp")

add_subdirectory("${CMAKE_CURRENT_SOURCE_DIR}/Sandbox/Engine/Hypershock")

set(HYPERSHOCK_BUILD_TYPE "STATIC")

target_link_libraries(Hypershock-Game Hypershock)
