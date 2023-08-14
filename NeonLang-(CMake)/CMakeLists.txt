cmake_minimum_required(VERSION 3.19)
project(main C CXX)
set(CMAKE_CXX_STANDARD 17)
# set(CMAKE_CXX_FLAGS "-m32")

# 输出操作系统平台信息
math(EXPR TARGET_BITS "8 * ${CMAKE_SIZEOF_VOID_P}")
if (WIN32)
    message(STATUS "Building on Windows platform.")
elseif (APPLE)
    message(STATUS "Building on MacOS platform.")
    add_compile_definitions(TARGET_OS_MAC)
elseif (UNIX)
    message(STATUS "Building on UNIX-like OS platform.")
elseif (MinGW)
    message(STATUS "Building on UNIX-like OS platform.")
endif ()

include_directories(include)


# 添加头文件(*/include)
include_directories(NeonLang/include)
include_directories(demo/include)

# 添加创建库文件的子目录
add_subdirectory(Neon)
add_subdirectory(demo)