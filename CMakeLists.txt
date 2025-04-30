cmake_minimum_required(VERSION 3.29.0)#先定义最小cmake版本号

project(
    Cmakeproject
    VERSION 0.0.1
    DESCRIPTION "a demo of cmake planning"
    HOMEPAGE_URL "https://github.com/cmh0731/Cmakeproject"
    LANGUAGES CXX
) #对project进行详细的描述，依次是文件名，版本号，描述，仓库地址，语言

set(CMAKE_CXX_STANDARD 17) #设置C++版本号

set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${PROJECT_SOURCE_DIR}/bin) #设置可执行文件exe和动态库的储存目录，这样做后子目录也可以用父目录的变量，相当于C++类与类的继承

add_subdirectory(src) #添加子目录