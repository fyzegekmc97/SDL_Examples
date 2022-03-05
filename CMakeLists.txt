cmake_minimum_required(VERSION 3.21)
project(SDL_Examples C)

set(CMAKE_C_STANDARD 11)

find_package(SDL2 REQUIRED)
include_directories(${SDL2_INCLUDE_DIRS})

add_executable(SDL_Examples main.c)

target_link_libraries(SDL_Examples ${SDL2_LIBRARIES} /home/feyzi/Packages/SDL2_image-2.0.5/.libs/libSDL2_image.a)
