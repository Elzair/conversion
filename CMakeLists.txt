cmake_minimum_required(VERSION 3.3)

project(boost_conversion)

add_library(boost_conversion INTERFACE)

target_include_directories(boost_conversion BEFORE INTERFACE ${CMAKE_CURRENT_SOURCE_DIR}/include)

install(TARGETS boost_conversion DESTINATION lib)
install(DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}/include/boost DESTINATION include)
