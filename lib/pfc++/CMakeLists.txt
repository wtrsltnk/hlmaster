cmake_minimum_required(VERSION 3.14 FATAL_ERROR)

project(pfc++)

add_library(pfcpp STATIC)

target_sources(pfcpp
    PRIVATE
        src/CInetAddress.cpp
        src/CStringBuffer.cpp
        src/PArgumentList.cpp
        src/PLogfile.cpp
        src/PSocket.cpp
        src/PString.cpp
        src/PStringList.cpp
        src/PUDPSocket.cpp
        include/pfc++/file.h
        include/pfc++/inet.h
        include/pfc++/socket.h
        include/pfc++/string.h
        include/pfc++/system.h
        include/pfc++/types.h
        include/CInetAddress.h
        include/CStringBuffer.h
        include/PArgumentList.h
        include/PException.h
        include/PFile.h
        include/PLogfile.h
        include/PSocket.h
        include/PString.h
        include/PStringList.h
        include/PUDPSocket.h
)
target_include_directories(pfcpp
    PUBLIC
        "./include"
    PUBLIC
        "./include"
)

