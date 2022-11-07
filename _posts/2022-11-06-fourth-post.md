---
layout: post
title: What are the CMake's Debug mode options?
tags: CMake
categories: build tools
---

We now know how to enable the *verbose* setting in CMakeLists.txt allowing us to view the **Debug** mode options.
And here they are,

`
[build] [7/14  14% :: 0.329] /usr/bin/g++  -I/home/amol/projects/github/cpp/x86_64/sensors/src -g -MD  
-MT sensors/CMakeFiles/sensors.dir/src/sensor.cpp.o   
-MF sensors/CMakeFiles/sensors.dir/src/sensor.cpp.o.d   
-o sensors/CMakeFiles/sensors.dir/src/sensor.cpp.o   
-c /home/amol/projects/github/cpp/x86_64/sensors/src/sensor.cpp
`
