cmake_minimum_required(VERSION 3.19)
project(merger CXX)

set(CMAKE_CXX_STANDARD 17)

add_executable(merger main.cpp buffer.h)
target_compile_features(merger PRIVATE cxx_std_17)

install(TARGETS merger RUNTIME DESTINATION ${CMAKE_INSTALL_BINDIR})