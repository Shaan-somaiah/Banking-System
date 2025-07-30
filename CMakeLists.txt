cmake_minimum_required(VERSION 3.10)

#add_compile_options(-ggdb -g -pedantic-errors -Wall -Weffc++ -Wextra -Wconversion -Wsign-conversion -Werror -std=c++14)

add_compile_options(-DNDEBUG -O2)

project (bankingSystem)

set (source_dir "${PROJECT_SOURCE_DIR}/")

file (GLOB source_files "${source_dir}/*.cpp")

add_executable(bankingSystem ${source_files})
