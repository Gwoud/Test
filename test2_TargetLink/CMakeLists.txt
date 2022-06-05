set(CMAKE_C_COMPILER "C:/Program Files (x86)/Dev-Cpp/MinGW64/bin/gcc.exe")
set(CMAKE_CXX_COMPILER "C:/Program Files (x86)/Dev-Cpp/MinGW64/bin/g++.exe")

project(demo)

add_library(thucai STATIC test.c test.h)
add_executable(demo main.c)
target_link_libraries(demo INTERFACE thucai)
