cmake_minimum_required(VERSION 3.10)
project(Project_Name)

file(GLOB_RECURSE SOURCES "Source/src/*.cpp")
file(GLOB_RECURSE HEADERS "Source/include/*.h")

add_executable(MyAPP ${SOURCES} ${HEADERS})