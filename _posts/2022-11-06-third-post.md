---
layout: post
title: How-to update VSCode CMake build args?
tags: CMake
categories: build tools
---

In the previous post we looked at what VSCode does with CMake with default settings.
It is assumed that we have installed the appropriate extensions for CMake & CMake Tools.

We found that we can select **Debug** or **Release** mode for our builds, but have no idea what flags constitute these modes.
In order to find what flags CMake applies for these mode, we need to add **VERBOSE=1** argument to the **build** command.

This can be done in multiple ways,
1. `set(CMAKE_VERBOSE_MAKEFILE ON)` : adding this to the CMakeLists.txt file enable verbosity on that particular tree node, but is not passed to other CMakeLists.txt files.
2. Update settings in **CMake Tools** extension.
   - Find **Cmake: Build Tool Args** : click **Add Item**, enter `--verbose`

**NOTE**: we need to delete the *build* folder and redo the *Configure* and *build* steps to see the verbose output.
