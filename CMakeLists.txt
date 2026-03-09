cmake_minimum_required(VERSION 3.28)
project(MyProject VERSION 1.0 LANGUAGES CXX)

find_package(Boost REQUIRED COMPONENTS filesystem)

add_executable(app main.cpp)

target_link_libraries(app PRIVATE Boost::filesystem)
