cmake_minimum_required(VERSION 3.16)

add_executable(main main.c)

find_package(unofficial-sqlite3 CONFIG REQUIRED)
target_link_libraries(main PRIVATE unofficial::sqlite3::sqlite3)