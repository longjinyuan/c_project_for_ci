cmake_minimum_required (VERSION 3.0)
project (c_project_for_ci)

set (CTEST_PROJECT_NAME "c_project_for_ci")
set (CMAKE_CXX_STANDARD 11)

#include_directories (/usr/local/include)
#link_directories (/usr/local/lib)

file (GLOB_RECURSE srcs src/*.cpp src/*.c src/*.cc src/*.h src/*.hpp)

add_executable (c_project_for_ci ${srcs})

#target_link_libraries (c_project_for_ci dl pthread m z)

## add the install targets
#install (DIRECTORY bin/ DESTINATION /data/app/c_project_for_ci/bin)
#install (DIRECTORY etc/ DESTINATION /data/app/c_project_for_ci/etc)
