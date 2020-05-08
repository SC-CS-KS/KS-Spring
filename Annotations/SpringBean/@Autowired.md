# @Autowired

标记Spring将要解析和注入的依赖项。  

```text
作用于构造函数
作用于setter方法
作用于字段
```

## 源码解析

```java
@Target({ElementType.CONSTRUCTOR, ElementType.FIELD, ElementType.METHOD, ElementType.ANNOTATION_TYPE})
@Retention(RetentionPolicy.RUNTIME)
@Documented
public @interface Autowired {
 /**
 * Declares whether the annotated dependency is required.
 * <p>Defaults to {@code true}.
 */
 boolean required() default true;
}
```

* 注解处理器  

org.springframework.context.annotation.internalAutowiredAnnotationProcessor  
对应于AutowiredAnnotationBeanPostProcessor  




