project(STB)

file(GLOB STB_SRC "*.h")

add_library(STB INTERFACE)
add_library(STB INTERFACE ${STB_SRC})

target_sources(STB INTERFACE ${STB_SRC})

target_include_directories(STB INTERFACE src)
