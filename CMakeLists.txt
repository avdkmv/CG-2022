cmake_minimum_required(VERSION 3.2)

project(CG)

find_package(VTK REQUIRED)
find_package(ITK REQUIRED)

add_executable(CG ./src/source.cpp)
target_link_libraries(CG ${VTK_LIBRARIES})
target_link_libraries(CG ${ITK_LIBRARIES})