cmake_minimum_required( VERSION 3.16.3 )

project(
    Hello_Cmake
    VERSION 0.1.0
    DESCRIPTION "Hello Cmake!!"
    LANGUAGES CXX
)

add_executable(${PROJECT_NAME}
    main.cpp
)