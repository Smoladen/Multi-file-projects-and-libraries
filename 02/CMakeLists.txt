cmake_minimum_required(VERSION 3.5)

project(02 LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_executable(02 src/main.cpp
    class/counter.cpp
    class/counter_classes.h)

include(GNUInstallDirs)
install(TARGETS 02
    LIBRARY DESTINATION ${CMAKE_INSTALL_LIBDIR}
    RUNTIME DESTINATION ${CMAKE_INSTALL_BINDIR}
)
