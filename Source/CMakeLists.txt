cmake_minimum_required(VERSION 2.8)

PROJECT(Skel3D)

find_package(ITK REQUIRED)
include(${ITK_USE_FILE})

add_executable(Skel3D BinaryThinning3D.cxx itkBinaryThinningImageFilter3D.h itkBinaryThinningImageFilter3D.cxx)

target_link_libraries(Skel3D ${ITK_LIBRARIES})
