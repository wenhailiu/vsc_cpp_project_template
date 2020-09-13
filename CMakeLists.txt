cmake_minimum_required(VERSION 3.8)
project(vscpp_project_template)

set(CXX_STANDARD 11)

#find third party libraries: 

# When there is no default VTK in your system folder, then you can specify the 
# build tree folder manually, then CMake will automatically configure all the 
# include dirs, lib dirs etc... For example: 
# set(VTK_DIR /Users/wl/Documents/packages/VTK/VTK-8.2.0/build)

# Let cmake find and configure all the required lib files: 
# find_package(VTK REQUIRED)
# include_directories(${VTK_INCLUDE_DIRS})

#Qt: 
# set(Qt5_DIR C:/Qt/Qt5.9.1/5.9.1/msvc2015/lib/cmake/Qt5)
# find_package(Qt5 COMPONENTS Core Widgets Xml OpenGL Network X11Extras REQUIRED)
# include_directories(${QT_INCLUDES})
# set(CMAKE_AUTOUIC ON)
# set(CMAKE_AUTOMOC ON)
# set(CMAKE_AUTORCC ON)

# OS specific instructions: 
if(UNIX)
endif(UNIX)

if(WIN32)
endif(WIN32)

if(APPLE)
endif(APPLE)

# Compile time definition: macros
# add_compile_definitions(SPDLOG_COMPILED_LIB)

# target: executable: 
add_executable(
    ExecutableName
    # src tree/*.cpp
    src/main.cpp
)

# link: 
target_link_libraries(
    ExecutableName
    # Libs, for example: 
    # ${VTK_LIBRARIES}
)