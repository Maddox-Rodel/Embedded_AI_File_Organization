cmake_minimum_required(VERSION 3.19)

project(File_Organizer LANGUAGES CXX)

find_package(Qt6 REQUIRED COMPONENTS Core Widgets)

qt_standard_project_setup()

qt_add_executable(File_Organizer
    main.cpp
    mainwindow.cpp
    mainwindow.h
    mainwindow.ui
)

target_link_libraries(File_Organizer
    PRIVATE
        Qt6::Core
        Qt6::Widgets
)