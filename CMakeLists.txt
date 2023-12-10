cmake_minimum_required(VERSION 3.10)
project(cxx-template)
set(SRC_DIR ${CMAKE_CURRENT_SOURCE_DIR}/src)
set(BINARY_DIR ${CMAKE_BINARY_DIR})
set(CMAKE_ARCHIVE_OUTPUT_DIRECTORY ${BINARY_DIR}/lib)
set(CMAKE_LIBRARY_OUTPUT_DIRECTORY ${BINARY_DIR}/lib)
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${BINARY_DIR}/bin)
add_executable(
	executable
	${SRC_DIR}/main.cxx
)
target_include_directories(
	executable
	PRIVATE
	${SRC_DIR}/include
)
