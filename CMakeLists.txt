cmake_minimum_required(VERSION 3.0.0)
project(template VERSION 0.1.0)

include_directories(${CMAKE_SOURCE_DIR}/include)

include(CTest)
enable_testing()

add_executable(template src/main.cpp include/main.h)

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)
