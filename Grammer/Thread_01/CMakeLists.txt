cmake_minimum_required(VERSION 3.5)

project(thread_01)

find_package(Threads)
set(CMAKE_CXX_STANDARD 11)

add_executable(thread_01 main.cpp)
target_link_libraries(thread_01 ${CMAKE_THREAD_LIBS_INIT})

add_executable(mutex mutex.cpp)
target_link_libraries(mutex ${CMAKE_THREAD_LIBS_INIT})

add_executable(mutex_02 mutex_02.cpp)
target_link_libraries(mutex_02 ${CMAKE_THREAD_LIBS_INIT})