qt5_hello_world
===============

``` bash
drasko@Lenin:~/qt/hello$ mkdir build

drasko@Lenin:~/qt/hello$ cd build/

drasko@Lenin:~/qt/hello/build$ cmake ..
-- The C compiler identification is GNU 4.9.1
-- The CXX compiler identification is GNU 4.9.1
-- Check for working C compiler: /usr/bin/cc
-- Check for working C compiler: /usr/bin/cc -- works
-- Detecting C compiler ABI info
- Detecting C compiler ABI info - done
-- Check for working CXX compiler: /usr/bin/c++
-- Check for working CXX compiler: /usr/bin/c++ -- works
-- Detecting CXX compiler ABI info
-- Detecting CXX compiler ABI info - done
-- Configuring done
-- Generating done
-- Build files have been written to: /home/drasko/qt/hello/build

drasko@Lenin:~/qt/hello/build$ make VERBOSE=1
/usr/bin/cmake -H/home/drasko/qt/hello -B/home/drasko/qt/hello/build --check-build-system CMakeFiles/Makefile.cmake 0
/usr/bin/cmake -E cmake_progress_start /home/drasko/qt/hello/build/CMakeFiles /home/drasko/qt/hello/build/CMakeFiles/progress.marks
make -f CMakeFiles/Makefile2 all
make[1]: Entering directory '/home/drasko/qt/hello/build'
make -f CMakeFiles/helloworld_automoc.dir/build.make CMakeFiles/helloworld_automoc.dir/depend
make[2]: Entering directory '/home/drasko/qt/hello/build'
cd /home/drasko/qt/hello/build && /usr/bin/cmake -E cmake_depends "Unix Makefiles" /home/drasko/qt/hello /home/drasko/qt/hello /home/drasko/qt/hello/build /home/drasko/qt/hello/build /home/drasko/qt/hello/build/CMakeFiles/helloworld_automoc.dir/DependInfo.cmake --color=
Dependee "/home/drasko/qt/hello/build/CMakeFiles/helloworld_automoc.dir/DependInfo.cmake" is newer than depender "/home/drasko/qt/hello/build/CMakeFiles/helloworld_automoc.dir/depend.internal".
Dependee "/home/drasko/qt/hello/build/CMakeFiles/CMakeDirectoryInformation.cmake" is newer than depender "/home/drasko/qt/hello/build/CMakeFiles/helloworld_automoc.dir/depend.internal".
Scanning dependencies of target helloworld_automoc
make[2]: Leaving directory '/home/drasko/qt/hello/build'
make -f CMakeFiles/helloworld_automoc.dir/build.make CMakeFiles/helloworld_automoc.dir/build
make[2]: Entering directory '/home/drasko/qt/hello/build'
/usr/bin/cmake -E cmake_progress_report /home/drasko/qt/hello/build/CMakeFiles 4
[ 25%] Automatic moc for target helloworld
/usr/bin/cmake -E cmake_autogen /home/drasko/qt/hello/build/CMakeFiles/helloworld_automoc.dir/ ""
AUTOGEN: Checking /home/drasko/qt/hello/main.cpp
AUTOGEN: Checking /home/drasko/qt/hello/hello.cpp
AUTOGEN: Checking /home/drasko/qt/hello/hello.hpp
Generating moc_hello.cpp
/usr/lib/x86_64-linux-gnu/qt5/bin/moc -I/home/drasko/qt/hello/build -I/home/drasko/qt/hello -I/usr/include/x86_64-linux-gnu/qt5 -I/usr/include/x86_64-linux-gnu/qt5/QtCore -I/usr/lib/x86_64-linux-gnu/qt5/mkspecs/linux-g++-64 -DQT_CORE_LIB -DQT_NO_DEBUG -o /home/drasko/qt/hello/build/moc_hello.cpp /home/drasko/qt/hello/hello.hpp 
make[2]: Leaving directory '/home/drasko/qt/hello/build'
/usr/bin/cmake -E cmake_progress_report /home/drasko/qt/hello/build/CMakeFiles  4
[ 25%] Built target helloworld_automoc
make -f CMakeFiles/helloworld.dir/build.make CMakeFiles/helloworld.dir/depend
make[2]: Entering directory '/home/drasko/qt/hello/build'
cd /home/drasko/qt/hello/build && /usr/bin/cmake -E cmake_depends "Unix Makefiles" /home/drasko/qt/hello /home/drasko/qt/hello /home/drasko/qt/hello/build /home/drasko/qt/hello/build /home/drasko/qt/hello/build/CMakeFiles/helloworld.dir/DependInfo.cmake --color=
Dependee "/home/drasko/qt/hello/build/CMakeFiles/helloworld.dir/DependInfo.cmake" is newer than depender "/home/drasko/qt/hello/build/CMakeFiles/helloworld.dir/depend.internal".
Dependee "/home/drasko/qt/hello/build/CMakeFiles/CMakeDirectoryInformation.cmake" is newer than depender "/home/drasko/qt/hello/build/CMakeFiles/helloworld.dir/depend.internal".
Scanning dependencies of target helloworld
make[2]: Leaving directory '/home/drasko/qt/hello/build'
make -f CMakeFiles/helloworld.dir/build.make CMakeFiles/helloworld.dir/build
make[2]: Entering directory '/home/drasko/qt/hello/build'
/usr/bin/cmake -E cmake_progress_report /home/drasko/qt/hello/build/CMakeFiles 1
[ 50%] Building CXX object CMakeFiles/helloworld.dir/main.cpp.o
/usr/bin/c++   -DQT_CORE_LIB -DQT_NO_DEBUG -Wall -fPIE -I/home/drasko/qt/hello/build -I/home/drasko/qt/hello -isystem /usr/include/x86_64-linux-gnu/qt5 -isystem /usr/include/x86_64-linux-gnu/qt5/QtCore -isystem /usr/lib/x86_64-linux-gnu/qt5/mkspecs/linux-g++-64    -o CMakeFiles/helloworld.dir/main.cpp.o -c /home/drasko/qt/hello/main.cpp
/usr/bin/cmake -E cmake_progress_report /home/drasko/qt/hello/build/CMakeFiles 2
[ 75%] Building CXX object CMakeFiles/helloworld.dir/hello.cpp.o
/usr/bin/c++   -DQT_CORE_LIB -DQT_NO_DEBUG -Wall -fPIE -I/home/drasko/qt/hello/build -I/home/drasko/qt/hello -isystem /usr/include/x86_64-linux-gnu/qt5 -isystem /usr/include/x86_64-linux-gnu/qt5/QtCore -isystem /usr/lib/x86_64-linux-gnu/qt5/mkspecs/linux-g++-64    -o CMakeFiles/helloworld.dir/hello.cpp.o -c /home/drasko/qt/hello/hello.cpp
/usr/bin/cmake -E cmake_progress_report /home/drasko/qt/hello/build/CMakeFiles 3
[100%] Building CXX object CMakeFiles/helloworld.dir/helloworld_automoc.cpp.o
/usr/bin/c++   -DQT_CORE_LIB -DQT_NO_DEBUG -Wall -fPIE -I/home/drasko/qt/hello/build -I/home/drasko/qt/hello -isystem /usr/include/x86_64-linux-gnu/qt5 -isystem /usr/include/x86_64-linux-gnu/qt5/QtCore -isystem /usr/lib/x86_64-linux-gnu/qt5/mkspecs/linux-g++-64    -o CMakeFiles/helloworld.dir/helloworld_automoc.cpp.o -c /home/drasko/qt/hello/build/helloworld_automoc.cpp
Linking CXX executable helloworld
/usr/bin/cmake -E cmake_link_script CMakeFiles/helloworld.dir/link.txt --verbose=1
/usr/bin/c++    -Wall    CMakeFiles/helloworld.dir/main.cpp.o CMakeFiles/helloworld.dir/hello.cpp.o CMakeFiles/helloworld.dir/helloworld_automoc.cpp.o  -o helloworld -rdynamic /usr/lib/x86_64-linux-gnu/libQt5Core.so.5.3.1 
make[2]: Leaving directory '/home/drasko/qt/hello/build'
/usr/bin/cmake -E cmake_progress_report /home/drasko/qt/hello/build/CMakeFiles  1 2 3
[100%] Built target helloworld
make[1]: Leaving directory '/home/drasko/qt/hello/build'
/usr/bin/cmake -E cmake_progress_start /home/drasko/qt/hello/build/CMakeFiles 0
drasko@Lenin:~/qt/hello/build$ 

drasko@Lenin:~/qt/hello/build$ ./helloworld 
Created Hello class!
Starting Hello daemon...
^C
drasko@Lenin:~/qt/hello/build$ 
```
# qt5GstreamerExample
