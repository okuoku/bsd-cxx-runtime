cmake_minimum_required(VERSION 2.8)

PROJECT(bsd-cxx-runtime)

include_directories(
    ${CMAKE_CURRENT_SOURCE_DIR}/libunwind/include
    ${CMAKE_CURRENT_SOURCE_DIR}/libunwind/include/tdep
    )

add_subdirectory(libunwind)
add_subdirectory(libcxx)
add_subdirectory(libcxxrt)
