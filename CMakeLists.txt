set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED True)

cmake_minimum_required(VERSION 3.30)
project(Gzhel VERSION 1.0)


include_directories(${PROJECT_SOURCE_DIR}/include)  
include_directories(${PROJECT_SOURCE_DIR}/libs/YourLibrary/include)

add_executable(Gzhel src/main.cpp)
