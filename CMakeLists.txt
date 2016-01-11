cmake_minimum_required(VERSION 3.3)
project(fb-inspect)
ADD_DEFINITIONS(

        -lGL
        -lGLU
        -lGLEW
        -lglfw
)


set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -Wall -Werror -std=c11")

set(SOURCE_FILES main.c )

add_executable(fb-inspect ${SOURCE_FILES})
target_link_libraries(fb-inspect GLEW GL GLU glfw)