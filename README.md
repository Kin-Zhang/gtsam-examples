GTSAM Tutorial Examples
===================================================
This repo is a collection of [GTSAM](https://bitbucket.org/gtborg/gtsam) tutorial examples for GTSAM starters by [Jing Dong](mailto:thu.dongjing@gmail.com). Checkout GTSAM tutorial slides for more explanations and infomation. 

2016年视频：[【泡泡机器人公开课】第五十六课：gtsam_tutorial-董靖B站](https://www.bilibili.com/video/BV1C4411772G)

此处新增python，对于python只需pip install即可，无需下列prerequisites，如果不想安装，推荐google colab进行简单尝试

```
pip3 install gtsam
```

---

以下为原readme中所含cpp和matlab所需

Prerequisites
------

- CMake >= 2.6 (Ubuntu: `sudo apt-get install cmake`), compilation configuration tool.
- [Boost](http://www.boost.org/) >= 1.50 (Ubuntu: `sudo apt-get install libboost-all-dev`), portable C++ source libraries.
- [GTSAM](https://bitbucket.org/gtborg/gtsam) >= 4.0 alpha.

Compilation & Installation
------

In the library folder excute:

```
$ mkdir build
$ cd build
$ cmake ..
$ make
```

Matlab Toolbox
-----

An optional Matlab toolbox is provided to use our library in Matlab. To enable Matlab toolbox during compilation:

```
$ cmake -DEXAMPLES_BUILD_MATLAB_TOOLBOX:OPTION=ON -DGTSAM_TOOLBOX_INSTALL_PATH:PATH=/path/install/toolbox ..
$ make install
```

After you install the Matlab toolbox, don't forget to add `/path/install/toolbox` to your Matlab path.

Tested Compatibility
-----

The gpmp2 library is designed to be cross-platform, however it's only tested on Ubuntu Linux for now.

- Compilers: GCC 4.8, 4.9, 5.3
- Boost version: 1.50 - 1.60

