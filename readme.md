# Cross-Plateform CMake template - a simple template cmake project structure for GLEW and SFML

This directory structure allows to add in a simple way new third-party librarie editting the `CMakeLists.txt`
at the root directory and the one in `ext` folder. 

An example project has been setup to show an example with the open-source libraries GLEW and SFML.

[SFML - Simple and Fast Multimedia Library](https://www.sfml-dev.org/) <br />
[GLEW - The OpenGL Extension Wrangler Library](http://glew.sourceforge.net/) <br />

## Authors

- Philippe Weier - (philippe.weier@epfl.ch)

## Install

- Make a new directory called build:
  `mkdir build`
- From the build directory run cmake:
  `cd build`
  `cmake ..`
- Finally build the whole project and it's dependencies
  `make`

## Changing project name

To change the executable's name change the following in the root `CMakeLists.txt`
`# Project name`
`project(YOUR_PROJECT_NAME)`

And all the other occurences of `YOUR_PROJECT_NAME` in the file.
