cmake_minimum_required(VERSION 2.8.3)
project(exercise_2)

# TODO invokes the routines to find a package called Eigen3
find_package(Eigen3)
# TODO specify additional locations of header files
include_directories(
    ${EIGEN3_INCLUDE_DIR}
    $(PROJECT_SOURCE_DIR)/src
)
# add project source code
add_subdirectory(src)
# TODO do the same for executables
