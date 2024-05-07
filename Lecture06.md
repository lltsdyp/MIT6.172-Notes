# 第六讲 多核处理器上的编程

## 几种常见的并发框架
* **pthread/WinAPI**
* **TBB(Thread Building Blocks)**
* **OpenMP**
* **Cilk**

## pthread/WinAPI
这两个库分别为\*nix系统和windows系统提供了系统API层级的并发支持，因此使用起来较为麻烦。

## TBB
TBB是由Intel推出的一款C++的并发编程库，将程序分解成一个个“任务”(task)，使用算法自动调度来尽可能的优化性能。

## OpenMP
OpenMP是一个支持C/C++和Fortran语言的库，它对并发的支持主要是通过编译器选项实现的（如C++中的`#pragma`预处理指令）。

## Cilk
Cilk是一个由本课程教师Charles Leiserson参与的并发编程框架，同时获得了Intel的支持，现在脱离Intel形成了[OpenCilk项目](https://github.com/OpenCilk/opencilk-project)
