# Spring Doc


## 标准 OpenAPI 文档

```xml
<dependency>
            <groupId>org.springdoc</groupId>
            <artifactId>springdoc-openapi-webflux-ui</artifactId>
            <version>1.3.0</version>
</dependency>
```

对应的Controller方法上添加一下@Operation进行说明:

```java
    @GetMapping("/nick/{id}")
    @Operation(description = "find nick by id")
    public Mono<String> findNickById(@PathVariable("id") Integer id) {
        return Mono.just("nick: " + 1);
    }
```

访问 http://xxxx:8080/swagger-ui.html   



