cmake_minimum_required (VERSION 3.4.3)

set(TARGET
    "valid-number"
    )

project(${TARGET}
    VERSION 1.0.0
    LANGUAGES "C"
    )

include(CMakeBase.inc)

set(SOURCES
    ${TARGET}.c
    )

set(DEPENDENCIES_LIST
    )

link_directories(
    )

include_directories(
    )

add_compile_options(
    -g
    )

add_definitions(
    )

add_executable(${TARGET}
    "${SOURCES}"
)

install(TARGETS ${TARGET}
    RUNTIME         DESTINATION bin
    )

target_link_libraries(${TARGET} "${DEPENDENCIES_LIST}")

set(CMAKE_EXPORT_COMPILE_COMMANDS ON)
#set(CMAKE_VERBOSE_MAKEFILE ON)
