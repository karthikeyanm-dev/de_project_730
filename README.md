# Demo1 - Spring Boot Application

A basic Spring Boot application created using Maven. This project follows the standard Spring Boot project structure with separate source code, resources, test code, and Maven build files.

## Project Structure

```text
demo1/
├── .idea/
├── .mvn/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/example/demo/
│   │   │       └── Demo1Application.java
│   │   └── resources/
│   │       └── application.properties
│   │
│   └── test/
│       └── java/
│           └── com/example/demo/
│               └── Demo1ApplicationTests.java
│
├── target/
├── .gitattributes
├── .gitignore
├── HELP.md
├── mvnw
├── mvnw.cmd
└── pom.xml
```

## Technologies

- Java
- Spring Boot
- Maven
- JUnit / Spring Boot Test
- IntelliJ IDEA

## Main Application

The application entry point is:

```text
src/main/java/com/example/demo/Demo1Application.java
```

This class contains the `main()` method used to start the Spring Boot application.

A typical Spring Boot main class looks like:

```java
package com.example.demo;

import org.springframework.boot.SpringApplication;
import org.springframework.boot.autoconfigure.SpringBootApplication;

@SpringBootApplication
public class Demo1Application {

    public static void main(String[] args) {
        SpringApplication.run(Demo1Application.class, args);
    }
}
```

## Configuration

Application configuration is maintained in:

```text
src/main/resources/application.properties
```

This file can be used to configure properties such as:

- Server port
- Database connection
- Application name
- Logging
- Spring Boot configuration

Example:

```properties
spring.application.name=demo1
server.port=8080
```

## Testing

The test class is located at:

```text
src/test/java/com/example/demo/Demo1ApplicationTests.java
```

Tests can be used to verify that the Spring application context loads successfully and to add unit or integration tests as the project grows.

Example:

```java
package com.example.demo;

import org.junit.jupiter.api.Test;
import org.springframework.boot.test.context.SpringBootTest;

@SpringBootTest
class Demo1ApplicationTests {

    @Test
    void contextLoads() {
    }
}
```

## Running the Application

### Using Maven Wrapper on Windows

Open a terminal in the project directory and run:

```cmd
mvnw.cmd spring-boot:run
```

### Using Maven Wrapper on Linux/macOS

```bash
./mvnw spring-boot:run
```

### Using IntelliJ IDEA

1. Open the project in IntelliJ IDEA.
2. Navigate to `Demo1Application.java`.
3. Click the Run button next to the `main()` method.
4. The Spring Boot application will start.

By default, the application is expected to run on:

```text
http://localhost:8080
```

## Building the Project

Using Windows:

```cmd
mvnw.cmd clean package
```

Using Linux/macOS:

```bash
./mvnw clean package
```

The compiled build output will be generated inside the `target/` directory.

## Important Directories

| Directory/File | Purpose |
|---|---|
| `src/main/java` | Application Java source code |
| `src/main/resources` | Configuration and application resources |
| `src/test/java` | Test source code |
| `pom.xml` | Maven project configuration and dependencies |
| `.mvn/` | Maven Wrapper configuration |
| `mvnw` | Maven Wrapper for Linux/macOS |
| `mvnw.cmd` | Maven Wrapper for Windows |
| `target/` | Generated build output |
| `application.properties` | Spring Boot application configuration |

## Future Development

This project can be extended by adding:

- REST Controllers
- Service classes
- Repository classes
- Entity classes
- Database connectivity
- Exception handling
- Validation
- Unit and integration tests
- Spring Data JPA
- Spring Security

## Author

Demo Spring Boot Project
