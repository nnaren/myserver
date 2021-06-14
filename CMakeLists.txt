cmake_minimum_required(VERSION 3.8)
Set(This MyServer)
project(${This} CXX)


add_subdirectory(reactor)
add_subdirectory(test)
