**原子类第一章 20200703**
<br>**AtomicBoolean**
<br>**1.0 重要属性**
<br>**1.0.1 sun.misc.Unsafe unsafe**
<br>**1.0.2 who?**
http://hg.openjdk.java.net/jdk8u/jdk8u60/hotspot/file/37240c1019fd/src/share/vm/prims/unsafe.cpp
<br>
<br>https://my.oschina.net/u/2518341/blog/1931106
<br>根据openjdk描述内容主要分为以下几点：
//todo
*  
*  
*
**1.0.3 why?**
<br> 为了解决线程的线程安全的问题，unsafe用了内存屏障技术，本质上
是乐观锁，判断当前值与期望值是否一致，如果一致则返回，否则则while循环自旋

**1.1 long valueOffset?**
<br>字面理解是值偏移量，从整体上来看这么设置是由于：


<br>2.0 重要方法
<br>3.0 适用场景