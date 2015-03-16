# Qt5 Gstreamer Example
## General Instructions
1. Install Qt Gstreamer from the source:
  - http://gstreamer.freedesktop.org/modules/qt-gstreamer.html
  - Add `-DQT_VERSION=5` compilation flag, as here: http://cgit.freedesktop.org/gstreamer/qt-gstreamer/tree/README#n88
2. Follow the doc here: http://gstreamer.freedesktop.org/data/doc/gstreamer/head/qt-gstreamer/html/build_system_integration.html to link with libraries like here: http://cgit.freedesktop.org/gstreamer/qt-gstreamer/tree/examples/appsink-src/CMakeLists.txt#n21
3. If needed, copy locally folder with `cmake` modules: http://cgit.freedesktop.org/gstreamer/qt-gstreamer/tree/cmake/modules and add them to `CMakeLists.txt` as exmplained here: https://github.com/rpavlik/cmake-modules with `list(APPEND CMAKE_MODULE_PATH "${CMAKE_CURRENT_SOURCE_DIR}/cmake/modules")`
4. Profit: `./soundlink mySong.mp3`

## Qt5 Build Instructions
```
drasko@Lenin:~/qt5/qt5GstreamerExample$ mkdir build
drasko@Lenin:~/qt5/qt5GstreamerExample$ cd build/
drasko@Lenin:~/qt5/qt5GstreamerExample/build$ cmake ..
-- The C compiler identification is GNU 4.9.2
-- The CXX compiler identification is GNU 4.9.2
-- Check for working C compiler: /usr/bin/cc
-- Check for working C compiler: /usr/bin/cc -- works
-- Detecting C compiler ABI info
-- Detecting C compiler ABI info - done
-- Check for working CXX compiler: /usr/bin/c++
-- Check for working CXX compiler: /usr/bin/c++ -- works
-- Detecting CXX compiler ABI info
-- Detecting CXX compiler ABI info - done
-- Boost hasn't been found yet. Looking...
-- Boost version: 1.55.0
-- GCC 4.5 or later detected. Enabling C++0x support in QTGSTREAMER_FLAGS.
-- Configuring done
-- Generating done
-- Build files have been written to: /home/drasko/qt5/qt5GstreamerExample/build
drasko@Lenin:~/qt5/qt5GstreamerExample/build$ make -j 8
Scanning dependencies of target soundlink
[100%] Building CXX object CMakeFiles/soundlink.dir/main.cpp.o
Linking CXX executable soundlink
[100%] Built target soundlink
drasko@Lenin:~/qt5/qt5GstreamerExample/build$ ./soundlink ~/audio/BobMarley-Jamming.mp3 
```
