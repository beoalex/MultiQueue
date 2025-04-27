
cmake_minimum_required(VERSION 3.8)

project("MultiQueue")

add_executable(${PROJECT_NAME} "Core.hpp" "Decls.hpp" "Processor.hpp" "UnitTests.cpp")

if(CMAKE_VERSION VERSION_GREATER 3.12)
    set_target_properties(${PROJECT_NAME} PROPERTIES CXX_STANDARD 20)
endif()

set_target_properties(${PROJECT_NAME} PROPERTIES OUTPUT_NAME "multi_queue")
