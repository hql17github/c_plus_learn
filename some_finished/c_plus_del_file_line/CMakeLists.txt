cmake_minimum_required(VERSION 3.10)  # 必须
set(CMAKE_CXX_STANDARD 11)	# C++14

project(cut_line)  #工程名

include_directories("/usr/local/include/") # 头文件目录

link_directories("/usr/local/lib/") # 链接库目录

aux_source_directory(. SRCS) # 源文件

add_executable(${PROJECT_NAME} ${SRCS}) # 生成可执行文件，这里程序名即为功能名

#target_link_libraries(${PROJECT_NAME} pthread) # 链接库

