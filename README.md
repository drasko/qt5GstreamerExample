# Qt5 Gstreamer Example
1. Install Qt Gstreamer from the source:
  - http://gstreamer.freedesktop.org/modules/qt-gstreamer.html
  - Add `-DQT_VERSION=5` compilation flag, as here: http://cgit.freedesktop.org/gstreamer/qt-gstreamer/tree/README#n88
2. Follow the doc here: http://gstreamer.freedesktop.org/data/doc/gstreamer/head/qt-gstreamer/html/build_system_integration.html to link wih libraries like here: http://cgit.freedesktop.org/gstreamer/qt-gstreamer/tree/examples/appsink-src/CMakeLists.txt#n21
3. If needed, copy locally folder with `cmake` modules: http://cgit.freedesktop.org/gstreamer/qt-gstreamer/tree/cmake/modules and add them to `CMakeLists.txt` as exmplained here: https://github.com/rpavlik/cmake-modules with `list(APPEND CMAKE_MODULE_PATH "${CMAKE_CURRENT_SOURCE_DIR}/cmake/modules")`
4. Profit
