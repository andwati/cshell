cmake_minimum_required(VERSION 3.31)

project(cshell VERSION 1.0 LANGUAGES C)

add_executable(cshell src/main.c)

set_property(TARGET cshell PROPERTY C_STANDARD 11)
set_property(TARGET cshell PROPERTY C_STANDARD_REQUIRED ON)

target_compile_options(cshell PRIVATE -Wall -Wextra -pedantic)

install(TARGETS cshell DESTINATION bin)
