cmake_minimum_required(VERSION 2.8)
project(CMakeHelloWorld)

#version number
set(CMakeHelloWorld_VERSION_MAJOR 1)
set(CMakeHelloWorld_VERSION_MINOR 0)

#find lib
set(ENV{PKG_CONFIG_PATH} "/opt/install/lib/pkgconfig")
FIND_PACKAGE(PkgConfig)
pkg_check_modules(HELLOLIB helloLib)


#add subdirectory
add_subdirectory(src)
