# 什么是依赖注入？

指 Spring 创建对象的过程中，将对象依赖属性（简单值，集合，对象）通过配置设值给该对象。
平常的Java开发中，程序员在某个类中需要依赖其它类的方法，则通常是new一个依赖类再调用类实例的方法，  
Spring提出了依赖注入的思想，即依赖类不由程序员实例化，而是通过Spring容器帮我们new指定实例并且将实例注入到需要该对象的类中。

在控制反转的基础上更进一步。
如果没有依赖注入，容器创建实例并保存后，调用者需要使用 getBean(String beanName) 才能获取到实例。
使用依赖注入时，容器会将 Bean 实例自动注入到完成相应配置的调用者，供其进一步使用。


## vs IoC

IoC 和 DI 其实是同一个概念的不同角度描述
DI 相对 IoC 而言，明确描述了“被注入对象依赖 IoC 容器配置依赖对象”。

依赖注入的另一种说法是“控制反转”，通俗的理解是：  
平常我们new一个实例，这个实例的控制权是我们程序员，而控制反转是指new实例工作不由我们程序员来做而是交给Spring容器来做。  