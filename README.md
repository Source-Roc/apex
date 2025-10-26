# Introduction

这个是我针对我的系统修改过的apex，修改如下:

- 1、全面 删除了 VERSION_GE_1_1/1_3/1_5 定义
- 2、修改 Tensor.type() => Tensor.options()
- 3、针对有在 [`mlp.cpp`](./csrc/mlp.cpp) 中有使用inputs.size() 作为for循环的判断条件时，同时使用 unsigned long 定义`unsigned long i`，删除了相关警告

原项目地址为：[NVIDIA/apex](https://github.com/NVIDIA/apex)

原项目README为：[README](./README-Origin.md)