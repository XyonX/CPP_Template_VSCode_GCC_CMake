cmake_minimum_required(VERSION 3.10)
project(Project_Name)

set(CMAKE_MAKE_PROGRAM "c:/msys64/usr/bin/make.exe")
set(CMAKE_GENERATOR "Unix Makefiles")

file(GLOB_RECURSE SOURCES "Source/src/*.cpp")
file(GLOB_RECURSE HEADERS "Source/include/*.h")

add_executable(MyAPP ${SOURCES} ${HEADERS})
target_include_directories(MyAPP PRIVATE "Source/include")

set(CMAKE_PREFIX_PATH "C:/Libraries/vcpkg/installed")