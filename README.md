# AOS project

## 裁剪内核
配置可以参考config文件
kernel is 815k

## Kernel Mode Linux

运行根目录下的程序a.out
通过gdb使得程序在main函数时中断

![user](user.png)

通过CS和SS的DPL=3可以看出是处于用户态

而/trusted目录下的a.out文件以内核态执行
![kernel](kernel.png)

可以看到DPL=0是内核态
