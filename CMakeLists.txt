cmake_minimum_required(VERSION 2.8.9)
project (uvc-exposure)
add_executable(uvc-exposure uvc-exposure.c)
target_link_libraries(uvc-exposure uvc)
