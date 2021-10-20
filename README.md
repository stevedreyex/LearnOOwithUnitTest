# LearnOOwithUnitTest
Find a better way to learn OOP? Why not try writing UnitTest!

## Main Goal
in this repo/project I'll demonstrate
- How to write UnitTest
- How to Implement the OO-Concept into our code
- And so on....

## Overview

1. [BasicUnitTest](./BasicUnitTest)
## Environment
- OS: MacOS Catalina 15.6
- Text Editor: Visual Studio Code

- To Execute, Please do the following steps:

1. Make sure you have already install [XCode](https://itunes.apple.com/tw/app/xcode/id497799835?l=en&mt=12) 

2. Open it until you see the welcome screen, then close it.

3. Execute following command in terminal to install [Homebrew](https://brew.sh/index_zh-tw).

```
$ /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

1. Download [googletest-release-1.8.0.zip](https://github.com/google/googletest/archive/release-1.8.0.zip) to your ~/Downloads directory.

2. Execute the following command to install google test library:
```
$ brew install cmake
$ cd ~/Downloads/googletest-release-1.8.0/googletest
$ mkdir build
$ cd build
$ cmake -Dgtest_build_samples=ON -Dgtest_build_tests=ON ~/Downloads/googletest-release-1.8.0/googletest
$ make
$ sudo mkdir /usr/local/Cellar/gtest
$ sudo cp ~/Downloads/googletest-release-1.8.0/googletest/build/libgtest.a /usr/local/Cellar/gtest/
$ sudo ln -snf /usr/local/Cellar/gtest/libgtest.a /usr/local/lib/libgtest.a
$ sudo cp -r ~/Downloads/googletest-release-1.8.0/googletest/include /usr/local/Cellar/gtest/
$ ln -snf ../Cellar/gtest/include/gtest /usr/local/include/gtest
```
6. For a faster way to execute these commands, please execute [setup.sh](/setup.sh)