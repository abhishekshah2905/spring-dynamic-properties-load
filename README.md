# Dynamic Properties Load Application

This Spring Boot application demonstrates how to load and manage properties dynamically at runtime.

## Overview
The application includes a DynamicEnvironmentProperties class that extends DynamicResourceLoader to load properties from a specified location and update them based on a specified update frequency.

## Getting Started

### Prerequisites
- Java JDK 8 or higher
- Maven
### Installation
1. Clone the repository:
```bash
  git clone https://github.com/abhishekshah2905/spring-dynamic-properties-load.git
```
2. Navigate to the project directory:
```bash
  cd spring-dynamic-properties-load
```
3. Build the project:
```bash
  mvn clean install
```
4. Run the application:
```bash
  mvn spring-boot:run
```
5. Access the application at http://localhost:8090

### Usage
- The HomeController class includes a / endpoint that displays the values of dynamically loaded properties.
- The application uses @Scheduled to update the properties at a specified interval.


###Configuration
- The application.properties file includes configuration for the server port and properties file path.
- The PropertiesConfigurer class loads properties from the specified file path using DynamicEnvironmentProperties.