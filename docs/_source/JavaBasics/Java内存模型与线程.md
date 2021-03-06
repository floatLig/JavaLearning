# 1. 概述

我们越来越希望计算机能够并发的执行多个任务，不仅仅是因为现代的`计算机CPU运算能力很厉害`，还有一个重要的原因是计算机的`处理速度比磁盘IO、网络通信、数据库访问快太多`。

衡量一个服务器性能高低好坏，一个重要的指标是`TPS`（每秒事务处理数）。但是，高的TPS，或者说，并发执行多个任务，会带来很多问题：`多个线程如何正确存取共享数据`，怎么样才能避免死锁等等。

- 缓存一致性
- MESI
- 内存模型
- 乱序排序、指令重排序
- 🤚 Java内存模型
- 内存间交互的操作
- 聊一下volatile
- 原子性、有序性、可见性
- Java线程、协程、状态转换

<br><br>

- Java是怎么保证线程安全的
- 那你介绍一下synchronized
- CAS
- ThreadLocal：<https://juejin.im/post/5ac2eb52518825555e5e06ee#heading-8>
- 锁优化：

```
轻量级锁
重量级锁

可重入锁

公平锁
非公平锁

乐观锁
悲观锁
```