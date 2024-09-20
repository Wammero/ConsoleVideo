cmake_minimum_required(VERSION 3.10)
project(CVMediaPlayer)

find_package(Curses REQUIRED)
find_package(OpenCV REQUIRED)

add_executable(CVMediaPlayer CVMediaPlayer.cpp)

target_link_libraries(CVMediaPlayer ${CURSES_LIBRARIES} ${OpenCV_LIBS})
