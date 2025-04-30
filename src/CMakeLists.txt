project(main)

add_subdirectory(pnc_map)
add_subdirectory(process)

add_executable(${PROJECT_NAME} main.cpp)#添加可执行文件

target_include_directories(${PROJECT_NAME}
PUBLIC
${CMAKE_SOURCE_DIR}/src/process
)
target_link_libraries(${PROJECT_NAME}
PUBLIC
process
)