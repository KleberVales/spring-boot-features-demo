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

## 📊 Fluxo de Inicialização do Spring Boot

```mermaid
flowchart TD
    A[Início da Aplicação] --> B[SpringApplication.run]
    B --> C[Spring Boot Auto-configuration]
    C --> D[Carregar Beans e Contexto]
    D --> E[Registrar HelloController]
    E --> F[Subir Tomcat embutido na porta 8081]
    F --> G[Aplicação Pronta para Requisições]
    G --> H[GET /hello → "Hello, Spring Boot!"]
    G --> I[GET /actuator/health → Status]
    G --> J[GET /actuator/info → Informações do App]
```


