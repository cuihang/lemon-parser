cmake_minimum_required(VERSION 3.24)
# 项目名称
project(lemon-parser)

message("开始编译 lemon-parser")

add_subdirectory(./src)
#set(CMAKE_CXX_STANDARD 17)

#add_library(lemon library.cpp)

# 编译完 开始执行
execute_process(COMMAND ./src/main
        RESULT_VARIABLE result_var
        ERROR_VARIABLE error_var)


message(STATUS "结束了 状态码是 ${result_var}")

message(STATUS "结束了 状态码是 ${error_var}")
#