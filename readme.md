# C++ Boilerplate
[![Build Status](https://travis-ci.org/Ytodi31/Valgrind.svg?branch=master)](https://travis-ci.org/YTodi31/Valgrind)

---

## Overview

Program to find errors using Valgrind and correct them.


## Standard install via command-line
```
git clone --recursive https://github.com/Ytodi31/Valgrind
cd <path to repository>
mkdir build
cd build
cmake ..
make
Run tests: ./test/cpp-test
Run program: ./app/shell-app
```

## Building for code coverage (for assignments beginning in Week 4)
```
sudo apt-get install lcov
cmake -D COVERAGE=ON -D CMAKE_BUILD_TYPE=Debug ../
make
make code_coverage
```
This generates a index.html page in the build/coverage sub-directory that can be viewed locally in a web browser.


## Outputs
Initial errors found using Valgrind are attached in text file - initialErrors.txt /n
Valgrind errors are corrected and output is attached in text file - finalErrors.txt /n
Output from memory profiler KCachegrind is attached as image - memoryProfileKcache.png
