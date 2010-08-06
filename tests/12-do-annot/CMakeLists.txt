# Test case for the CMake/OCaml project

# Descriptions: testcase for annotations

cmake_minimum_required( VERSION 2.6 )
set( CMAKE_MODULE_PATH ${CMAKE_SOURCE_DIR}/../.. )

project( 12-do-annot NONE )

find_package( OCaml REQUIRED )
include( UseOCaml )

add_ocaml_executable( foo
    SOURCES foo main
    OCAMLCOPTS -annot
    )
