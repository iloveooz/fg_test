cmake_minimum_required(VERSION 2.6)
project ("FG test")

add_definitions("-std=c++11")

set(CMAKE_BUILD_TYPE Debug)

set(SRC src/main.cpp
		src/Game.cpp
		src/Window.cpp
		src/WindowManager.cpp)

add_executable(fgwm.exe ${SRC})

target_link_libraries(fgwm.exe sfml-system)
target_link_libraries(fgwm.exe sfml-window)
target_link_libraries(fgwm.exe sfml-graphics)
target_link_libraries(fgwm.exe sfml-audio)
target_link_libraries(fgwm.exe sfml-network)
