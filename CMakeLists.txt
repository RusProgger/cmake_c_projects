cmake_minimum_required(VERSION 3.16)

project(new_projects LANGUAGES C)

add_executable(new_projects
    src/main.c
)

target_compile_features(new_projects PRIVATE c_std_11)

target_include_directories(new_projects PRIVATE
    ${CMAKE_SOURCE_DIR}/include
)

target_compile_options(new_projects PRIVATE
    -Wall
    -Wextra
    -Wpedantic
)