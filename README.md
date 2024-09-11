> 揭秘：从 Bash Shell 迁移 Zsh Shell的真正原因

# 什么是 shell

熟悉 Mac OS 的程序员都应该对 shell 有一定的了解。

在工作中，我们经常会使用一些 shell 命令来进行一些文件操作，比如下面这个 shell 命令：

```shell
# 在当前目录下创建了一个 learn 文件夹
mkdir learn
```

![alt text](image.png)

shell 是和系统内核指令打交道的一座桥梁。我们通过键盘输入一种自己容易记忆识别的符号标识（SHELL命令），有 SHELL解析这些命令再反馈给内核去执行一系列操作。

# shell类型

shell的类型分为很多种。不同的 shell 语法可能会有不同。

系统某些服务在运行过程中，会去检查用户能够使用的 shells，而这些 shells 的查询就是借助 /etc/shells 这个文件，使用 ```cat /etc/shells``` 命令查看当前系统支持哪些 SHELL脚本。

![alt text](image-1.png)

目前最常用的就是sh、 bash 和 zsh。接下来会重点说这 3 个。

## 常用的shell - sh

sh 是 shell 的缩写。

是 Unix/Linux 系统的默认 shell，也是最古老的 shell之一。

sh 是标准的 POSIX shell，有许多不同版本和实现，如 Bourne shell 和 POSIX shell。 

## 常用的shell - bash

bash全称是Bourne Again shell ，目前被绝大多数 Linux 系统所使用。

它是对Bourne shell的重新实现。

那么为什么要费劲巴拉的重新写一遍这个呢？这不是在重复造轮子嘛！

因为Bourne shell是Unix系统的一部分，自由软件之父Richard Stallman在1983年开始发起了GNU运动，GNU运动的目标是实现一个免费自由的操作系统，以解决Unix系统收费的一些限制。
