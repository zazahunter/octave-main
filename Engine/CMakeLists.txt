cmake_minimum_required(VERSION 3.16)

project(OctaveEngine)

file(GLOB_RECURSE OCTAVE_SOURCES Source/*.cpp Source/*.h)

add_library(${PROJECT_NAME} STATIC ${OCTAVE_SOURCES})

target_include_directories(${PROJECT_NAME} PUBLIC Source)

target_link_libraries(${PROJECT_NAME} PUBLIC glm vorbis STB)