cmake_minimum_required(VERSION 3.28.0)
project(Calc DESCRIPTION "un simple programa de calculadora" LANGUAGES CXX)

set(SRC_DIR ${PROJECT_SOURCE_DIR}/src)

add_executable(${PROJECT_NAME} ${SRC_DIR}/test-main.cpp ${SRC_DIR}/test.cpp)
target_include_directories(${PROJECT_NAME} PUBLIC ${PROJECT_SOURCE_DIR}/include)

target_link_libraries(Calc CATCH2)