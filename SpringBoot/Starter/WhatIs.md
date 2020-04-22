# What is Sprint Boot Starter?

Starter是Spring Boot中的一个非常重要的概念，Starter相当于模块，  
它能将模块所需的依赖整合起来并对模块内的Bean根据环境（ 条件）进行自动配置。  

使用者只需要依赖相应功能的Starter，无需做过多的配置和依赖，  
Spring Boot就能自动扫描并加载相应的模块。  

```text
1.它整合了这个模块需要的依赖库；
2.提供对模块的配置项给使用者；
3.提供自动配置类对模块内的Bean进行自动装配；
```

例如，  
在Maven的依赖中加入spring-boot-starter-web就能使项目支持Spring MVC，  
并且Spring Boot还为我们做了很多默认配置，无需再依赖spring-web、spring-webmvc等相关包及做相关配置就能够立即使用起来。
