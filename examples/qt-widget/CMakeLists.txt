cmake_minimum_required(VERSION 3.5)

project(qt-widget LANGUAGES CXX)

set(CMAKE_INCLUDE_CURRENT_DIR ON)

set(CMAKE_AUTOUIC ON)
set(CMAKE_AUTOMOC ON)
set(CMAKE_AUTORCC ON)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

find_package(Qt5 COMPONENTS Widgets REQUIRED)

add_executable(qt-widget
  main.cpp
  MainWindow.cpp
  MainWindow.hpp
  MainWindow.ui
)

target_link_libraries(qt-widget PRIVATE Qt5::Widgets)
