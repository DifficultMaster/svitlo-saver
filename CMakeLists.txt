cmake_minimum_required(VERSION 3.20)
project(SvitloSaver CXX)

set(CMAKE_CXX_STANDARD 23)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

set(JS_DIR "${CMAKE_CURRENT_SOURCE_DIR}/js")
set(SHARED_DIR "${CMAKE_CURRENT_SOURCE_DIR}/shared/proto")

add_subdirectory(cpp)