cmake_minimum_required(VERSION 3.25)

project(HelloWorld VERSION 1.0.0 LANGUAGES C CXX)

add_library(printHello STATIC myLib.cc)

add_executable(output main.cpp)

target_link_libraries(output PUBLIC printHello)