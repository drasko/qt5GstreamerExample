cmake_minimum_required(VERSION 2.8.11)

project(soundlink)

#list(APPEND CMAKE_MODULE_PATH "${CMAKE_CURRENT_SOURCE_DIR}/cmake/modules")

find_package( Qt5 COMPONENTS Core Gui Widgets REQUIRED)
find_package( Qt5GStreamer REQUIRED )
#find_package( GLIB2 )

# Find includes in the build directories
set(CMAKE_INCLUDE_CURRENT_DIR ON)


include_directories(${QTGSTREAMER_INCLUDES})
add_definitions(${QTGSTREAMER_DEFINITIONS})
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} ${QTGSTREAMER_FLAGS}")

# Tell CMake to create the helloworld executable
add_executable(soundlink main.cpp)

# Use the Core module from Qt5
target_link_libraries(soundlink ${QTGSTREAMER_UTILS_LIBRARIES})
