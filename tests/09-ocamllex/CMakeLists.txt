# Test case for CMake-OCaml

# Description: testcase for ocamllex

cmake_minimum_required( VERSION 2.6 )
set( CMAKE_MODULE_PATH ${CMAKE_SOURCE_DIR}/../.. )

project( 09-ocamllex )

find_package( OCaml REQUIRED )
include( UseOCaml )

add_ocaml_executable( count1
    SOURCES count.mll
    )

add_ocaml_executable( count2
    SOURCES count
    )
