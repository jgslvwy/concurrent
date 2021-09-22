jvm 知识
#1、什么情况下发生栈内存溢出： 
栈深度内存溢出： 
stackoverflowException: 主要是体现在局部变量表存储不下，比如递归调用。 
#2、JVM内存结构：  
堆（年轻代、老年代）、栈（虚机机栈、本地方法栈）、本地方法区、程序技术器、元空间（1.8改为元空间，为了解决堆区oom的问题，第二、与JRockit VM）  
垃圾回收的主要区域是堆区，主要有7种垃圾回收器：  
#3、垃圾回收器：  
serialNew，parilNew，serialOld，parilOld，parliNew，cms，g1：  
