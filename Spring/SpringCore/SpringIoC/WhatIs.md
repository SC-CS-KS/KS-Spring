# 什么是控制反转？

是一种设计思想，就是将原本在程序中手动创建对象的控制权，交由Spring框架来管理。

一般地，传统的程序设计中，无论是使用工厂创建实例，或是直接创建实例，实例调用者都要先主动创建实例，而后才能使用。
控制反转（Inverse of Control) 将实例的创建过程交由容器实现，调用者将控制权交出，是所谓控制反转。

* 正控 若要使用某个对象，需要自己去负责对象的创建
* 反控 若要使用某个对象，只需要从 Spring 容器中获取需要使用的对象

不关心对象的创建过程，也就是把创建对象的控制权反转给了Spring框架
* 好莱坞法则 - Don’t call me ,I’ll call you