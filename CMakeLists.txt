cmake_minimum_required(VERSION 3.22.1)

project(opengl)

add_subdirectory(external/glfw)

add_executable(main 
    app/main.cpp
    glad/src/glad.c
)

target_include_directories(main

    # PRIVATE external/glfw/include
    PRIVATE external/glm
    PRIVATE glad/include
)

target_link_libraries(main
    PRIVATE glfw
)