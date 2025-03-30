cmake_minimum_required(VERSION 3.20)

project(cs149 C CXX)

set(CMAKE_EXPORT_COMPILE_COMMANDS ON)
set(CMAKE_BUILD_TYPE Debug)
set(CMAKE_CXX_STANDARD_REQUIRED 20)

include_directories(${PROJECT_SOURCE_DIR}/asst1/common)

add_executable(prog1_mandelbrot_threads 
              ${PROJECT_SOURCE_DIR}/asst1/prog1_mandelbrot_threads/main.cpp 
              ${PROJECT_SOURCE_DIR}/asst1/prog1_mandelbrot_threads/mandelbrotThread.cpp
              ${PROJECT_SOURCE_DIR}/asst1/prog1_mandelbrot_threads/mandelbrotSerial.cpp)