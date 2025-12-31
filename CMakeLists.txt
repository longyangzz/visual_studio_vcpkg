# CMakeList.txt: helloworld 的 CMake 项目，在此处包括源代码并定义
# 项目特定的逻辑。
#
cmake_minimum_required (VERSION 3.8)

project(HelloWorld)

find_package(fmt CONFIG REQUIRED)

add_executable(HelloWorld helloworld.cpp)

target_link_libraries(HelloWorld PRIVATE fmt::fmt)
