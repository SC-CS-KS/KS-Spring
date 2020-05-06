# Spring Boot 配置

## 发展

* XML
  
在最初，Spring 使用 XML 配置文件的方式来描述 bean 的定义以及相互间的依赖关系  
所有业务类均以 bean 的形式配置在 XML 文件中，造成了大量的 XML 文件，使项目变得复杂且难以管理  
  
* Guice  

基于纯 Java Annotation 依赖注入框架，是一个轻量级 IOC 框架。  

* JavaConfig  

由于 Guice 带来的竞争压力，Spring 及社区推出并持续完善了 JavaConfig 子项目  
它基于 Java 代码和 Annotation 注解来描述 bean 之间的依赖绑定关系  

## 配置文件

般上来说，当我们创建一个SpringBoot项目时，IDE会默认帮我们创建一个application.properties配置文件。

### [application.properties](application.properties/README.md)

### [application.yml](application.yml/README.md)

### 比较

如果工程中同时存在application.properties文件和 application.yml文件，  
yml 文件会先加载，而后加载的properties文件会覆盖yml文件。  
所以建议工程中，只使用其中一种类型的文件即可。
