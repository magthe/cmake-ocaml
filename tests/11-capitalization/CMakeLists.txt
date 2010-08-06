# Test case for the CMake/OCaml project

# Descriptions: testcase 

cmake_minimum_required( VERSION 2.6 )
set( CMAKE_MODULE_PATH ${CMAKE_SOURCE_DIR}/../.. )

project( 11-capitalization NONE )

find_package( OCaml REQUIRED )
include( UseOCaml )

add_ocaml_executable( foo
    SOURCES fooBar main
    )
