cmake_minimum_required(VERSION 3.0)
project(ch4)

set(CMAKE_CXX_STANDARD 11)

# include_directories("/usr/include/eigen3")
find_package(Eigen3 3.3.0 REQUIRED)
message("Eigen3 Version: ${Eigen3_VERSION}")
include_directories(${EIGEN3_INCLUDE_DIR})
message("Include Dir: ${EIGEN3_INCLUDE_DIR}")
find_package(Pangolin REQUIRED)
include_directories(${Pangolin_INCLUDE_DIRS})

find_package(Sophus REQUIRED)
include_directories(${Sophus_INCLUDE_DIRS})
message("Sophus Include Dirs: ${Sophus_INCLUDE_DIRS}")

add_executable(useSophus useSophus.cpp)
add_executable(trajectoryError trajectoryError.cpp)
target_link_libraries(trajectoryError ${Pangolin_LIBRARIES})