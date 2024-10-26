set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED True)

cmake_minimum_required(VERSION 3.30)
project(Gzhel VERSION 1.0)

set(EXTERNAL_LIBRARIES_FOLDER ${CMAKE_SOURCE_DIR}/include)
set(CORE_SOURCE_FOLDER_NAME src)

add_subdirectory(engine/core)
add_subdirectory(include)
