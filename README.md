# 🌱 Spring Boot Features Demo

## Desafio:

- Criar uma aplicação simples com:
  - Spring Boot Starter Web
  - Endpoint /hello que retorna "Hello, Spring Boot!"
  - application.properties com customização (porta, nome da aplicação, etc.)
  - Adicionar Spring Boot Actuator e testar endpoints de monitoramento (/actuator/health, /actuator/info)
 
## 📂 Estrutura do Projeto

```text

spring-boot-features-demo/
 ├── build.gradle.kts
 ├── settings.gradle.kts
 └── src
     ├── main
     │   ├── java/com/example/features
     │   │   ├── SpringBootFeaturesDemoApplication.java
     │   │   └── controller/HelloController.java
     │   └── resources
     │       └── application.properties
     └── test/java/com/example/features
         └── SpringBootFeaturesDemoApplicationTests.java

```

## ▶️ Como Executar
Usando Gradle

```bash

./gradlew bootRun

```


