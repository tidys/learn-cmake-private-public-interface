cmake_minimum_required(VERSION 3.0.0)
project(app)
set(CMAKE_SKIP_RPATH TRUE)

include(./lib1/CMakeLists.txt)

# executable
add_executable(app ./app.cpp)

# linking
target_link_libraries(app PRIVATE lib1)