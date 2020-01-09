cmake_minimum_required(VERSION 3.3)
project(Lsn12_Example_race_cond)

set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -Wall -Werror")

set(SOURCE_FILES main.c)
add_executable(race_cond ${SOURCE_FILES})
target_link_libraries(race_cond pthread)