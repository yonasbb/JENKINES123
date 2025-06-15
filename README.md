# Jenkins JUnit Demo Project

This is a simple Java project that demonstrates the integration of Jenkins with JUnit testing. The project contains a basic Calculator class with its corresponding JUnit tests.

## Project Structure

```
├── src/
│   ├── main/java/com/example/
│   │   └── Calculator.java
│   └── test/java/com/example/
│       └── CalculatorTest.java
├── pom.xml
├── Jenkinsfile
└── README.md
```

## Prerequisites

- Java 11 or higher
- Maven 3.6 or higher
- Jenkins server with the following plugins:
  - Pipeline
  - JUnit
  - Maven Integration
  - Git Integration

## Local Development

1. Clone the repository
2. Run tests locally:
   ```bash
   mvn test
   ```
3. Build the project:
   ```bash
   mvn clean package
   ```

## Jenkins Setup

1. Create a new Pipeline job in Jenkins
2. Configure the job to use the Jenkinsfile from SCM
3. Set up the following tools in Jenkins:
   - JDK 11
   - Maven

## Pipeline Stages

The Jenkins pipeline includes the following stages:
1. Checkout - Gets the source code
2. Build - Compiles the code
3. Test - Runs JUnit tests
4. Package - Creates the final JAR file

## Test Coverage

The project includes unit tests for:
- Addition
- Subtraction
- Multiplication
- Division (including division by zero) # JENKINES123
