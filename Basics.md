# 📘 Spring Boot Notes

This repository contains my notes on **Spring Boot basics**.  
The goal is to maintain concise, practical references with examples.

---

## 🌱 Spring vs Spring Boot

- **Spring Framework**  
  - Provides comprehensive infrastructure support for developing Java applications.  
  - Requires manual configuration (XML or Java-based).  

- **Spring Boot**  
  - Built on top of Spring Framework.  
  - Provides **auto-configuration**, **embedded servers**, and **starter dependencies**.  
  - Reduces boilerplate code and setup time.  

---

## 🟦 @Bean

- Used to declare a bean in Spring’s application context.  
- Typically placed inside a `@Configuration` class.

```java
@Configuration
public class AppConfig {

    @Bean
    public MyService myService() {
        return new MyServiceImpl();
    }
}
