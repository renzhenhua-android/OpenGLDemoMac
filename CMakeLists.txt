cmake_minimum_required(VERSION 3.8)

project(Triangle)

include_directories(/opt/homebrew/Cellar/glfw/3.3.8/include
                    glad/include)

link_directories(/opt/homebrew/Cellar/glfw/3.3.8/lib)

add_executable(test main.cpp glad/src/glad.c)

target_link_libraries(test glfw)
