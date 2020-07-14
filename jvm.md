JVM 优化



1、为什么学JVM

2、JVM历史





程序计数器（唯一不会OOM的内存）

指向当前线程正在执行的字节码指令的地址（行号）

为什么需要程序计数器

1、java是多线程的，必然会有线程切换

2、确保多线程情况下的程序正常执行



栈

栈的数据结构

入口和出口只有一个

入栈和出栈

特点 现金后出  FILO

为什么JVM要使用栈？

虚拟机栈



泛型









内存溢出

java.lang.OutOfMemoryError: GC overhead limit exceeded







栈溢出

方法死循环递归调用(StackOverflowError)、不断建立线程(OutOfMemoryError)

不断创建对象，分配对象大于最大堆的大小(OutOfMemoryError)



OutOfMemoryError: GC overhead limit exceeded



OutOfMemoryError: Direct buffer memory 直接内存异常





内存泄漏

已经申请内存，但是无法释放已用的内存空间



