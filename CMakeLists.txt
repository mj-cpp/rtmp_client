cmake_minimum_required(VERSION 3.5.0)
project(rtmp_client VERSION 0.1.0 LANGUAGES C CXX)

file(GLOB_RECURSE SRC_FILES *.cc)
add_executable(rtmp_client ${SRC_FILES})

include(CTest)
enable_testing()

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)
