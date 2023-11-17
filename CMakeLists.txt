cmake_minimum_required(VERSION 3.25)

project(imgui)

file(GLOB IMGUI_SOURCES *.cpp)
file(GLOB IMGUI_HEADERS *.h)

add_library(imgui STATIC ${IMGUI_SOURCES} ${IMGUI_HEADERS})

target_include_directories(imgui PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})