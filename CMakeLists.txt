project(MeMessage C CXX)
cmake_minimum_required(VERSION 3.3.2)

include(cmake/App.cmake)

set (CMAKE_CXX_STANDARD 20)
set(SOURCES "src/logic/SocketCommunication.h"
            "src/logic/SocketCommunication.cpp"
            "src/UI/JavascriptInterop.h"
            "src/UI/JavascriptInterop.cpp"
            "src/MyApp.h"
            "src/MyApp.cpp"
            "src/main.cpp")

add_app("${SOURCES}")