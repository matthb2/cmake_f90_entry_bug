project(fortranpoc)
cmake_minimum_required(VERSION 3.0)

enable_language(Fortran)
enable_language(CXX)

add_executable(testprog test.f90)
set_target_properties(testprog PROPERTIES LINKER_LANGUAGE Fortran)
set_target_properties(testprog PROPERTIES HAS_CXX TRUE)
