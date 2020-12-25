# proj11-yet-another-coredump
### 项目名称
轻量级多处理器架构支持的 coredump 生成

### 项目描述

1. 为支持多种处理器架构（x86-64、risc-v、arm64）的Linux操作系统开发一个共享库，可以指定应用程序运行时候加载此库
2. 在应用程序崩溃时，这个库能自动生成当前用户态程序所有线程的调用栈信息，并将其保存在 coredump 文件里
3. coredump 文件是轻量级的，应比 Linux 内核生成的 coredump 要小至少一半
4. 生成的 coredump 文件可以被本地机器的 gdb 正常加载和分析 
5. 生成的 coredump 文件和崩溃程序的运行库信息可以拷贝到远程机器，在远程机器用 gdb 正常加载和分析

### 所属赛道

2021全国大学生操作系统比赛的“OS功能设计”赛道

### 参赛要求

- 以小组为单位参赛，最多三人一个小组，且小组成员是来自同一所高校的本科生（2021年春季学期或之后本科毕业的大一~大四的学生）
- 如学生参加了多个项目，参赛学生选择一个自己参加的项目参与评奖
- 请遵循“2021全国大学生操作系统比赛”的章程和技术方案要求

### 项目导师

**刘昌辉**

* github yy221

* email liuchanghui@uniontech.com

### 难度

中

### 特征

* 熟悉 elf 文件格式，elf 加载，elf 链接
* 熟悉 Linux 进程空间
* 熟悉 coredump 文件格式
* 熟悉 gdb 调试原理

### 参考项目

* gdb
* google breakpad

### License

* [GPL-3.0-only](https://opensource.org/licenses/GPL-3.0)

## 预期目标

### 注意：下面的内容是建议内容，不要求必须全部完成。选择本项目的同学也可与导师联系，提出自己的新想法，如导师认可，可加入预期目标

### 题目一

实现在本地机器的 gdb 正常加载和分析 coredump 文件

### 题目二

实现在远程机器上的 gdb 正常加载和分析 coredump 文件

