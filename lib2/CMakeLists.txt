add_library(lib2
    ${CMAKE_CURRENT_LIST_DIR}/lib2.h

    ${CMAKE_CURRENT_LIST_DIR}/lib2.cpp
)

target_include_directories(lib2 INTERFACE ${CMAKE_CURRENT_LIST_DIR})
