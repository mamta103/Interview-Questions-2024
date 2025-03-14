# Spring Boot Notes

## What is `@Bean` in Spring?
- `@Bean` is used to manually define a Spring-managed bean.
- It is placed inside a `@Configuration` class.
- Useful for **third-party libraries** that cannot use `@Component`.

## Example Usage:
```java
@Configuration
public class AppConfig {
    
    @Bean
    public MyService myService() {
        return new MyService(); // Bean definition
    }
}