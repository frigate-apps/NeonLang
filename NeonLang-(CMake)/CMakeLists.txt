cmake_minimum_required(VERSION 3.19)
project(demo C CXX)

include_directories(include)

file(GLOB APP_SOURCES source/*.cpp source/*.c)
# file(GLOB APP_HEADERS include/*.hpp include/*.h) ${APP_HEADERS}

# win32窗口、win32控制台
# add_executable(space-longan-renderer WIN32 source/main.cpp)

add_executable(demo ${APP_SOURCES})

# link_directories(
#    Neon
#)

# 添加链接库文件(lib)
target_link_libraries(demo
        # gcc
        # mingw32
        )