cmake_minimum_required(VERSION 3.14 FATAL_ERROR)

project(HLMaster)

add_subdirectory(lib/pfc++)

add_executable(HLMaster)

target_sources(HLMaster
    PRIVATE
        src/HLInfoList.cpp
        src/HLMaster.cpp
        src/HLServerFilterList.cpp
        src/HLServerList.cpp
        src/main.cpp
        include/HLInfoList.h
        include/HLMaster.h
        include/HLServerFilterList.h
        include/HLServerList.h
)
target_link_libraries(HLMaster
    PUBLIC
        pfcpp
        wsock32.lib
)
target_include_directories(HLMaster
    PUBLIC
        "./include"
        "lib/pfc++/include"
)
target_link_directories(HLMaster
    PUBLIC
        "lib/pfc++/Release"
    PUBLIC
        "lib/pfc++/Debug"
)

