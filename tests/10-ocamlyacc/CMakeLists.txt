# Test case for CMake-OCaml

# Description: testcase for ocamlyacc

cmake_minimum_required( VERSION 2.6 )
set( CMAKE_MODULE_PATH ${CMAKE_SOURCE_DIR}/../.. )

project( 10-ocamlyacc )

find_package( OCaml REQUIRED )
include( UseOCaml )

add_ocaml_executable( rpcalc1
    SOURCES lexer.mll rpcalc.mly main
    )

add_ocaml_executable( rpcalc2
    SOURCES lexer rpcalc main
    )
