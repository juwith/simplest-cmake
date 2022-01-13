cmake_minimum_required(VERSION 2.8)
project(CMakeHelloWorldLib)

#version number
set(CMakeHelloWorldLib_VERSION_MAJOR 1)
set(CMakeHelloWorldLib_VERSION_MINOR 0)

#add subdirectory
add_subdirectory(src)

configure_file(helloLib.pc.in ${CMAKE_INSTALL_PREFIX}/lib/pkgconfig/helloLib.pc @ONLY) 