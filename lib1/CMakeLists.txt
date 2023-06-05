include(${CMAKE_CURRENT_LIST_DIR}/../lib2/CMakeLists.txt)

add_library(lib1
    ${CMAKE_CURRENT_LIST_DIR}/lib1.h

    ${CMAKE_CURRENT_LIST_DIR}/lib1.cpp
)

target_include_directories(lib1 INTERFACE ${CMAKE_CURRENT_LIST_DIR})
target_link_libraries(lib1 PUBLIC lib2)
