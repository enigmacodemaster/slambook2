cmake_minimum_required(VERSION 2.8)
project(useSophus)
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11 ")
# find_package(Sophus REQUIRED)
# adapt my thinkpad-t480 env

set(EXECUTABLE_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/bin) # 把执行文件都写到工程目录下的bin文件夹底下
include_directories("/usr/local/include/")

# Eigen
include_directories("/usr/include/eigen3")
add_executable(useSophus useSophus.cpp)

add_subdirectory(example)
