cmake_minimum_required(VERSION 2.8)
project(rivlib-utils)

find_package(RiVLib COMPONENTS scanlib)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++0x")
set(EXECUTABLE_OUTPUT_PATH ${PROJECT_BINARY_DIR}/bin)

set (CMAKE_CXX_FLAGS "-m32")

include_directories(
    /home/vagrant/src/rimta-x86-linux-gcc47
    ${RiVLib_INCLUDE_DIRS}
    )

add_subdirectory(src)
