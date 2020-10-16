## Hexagonal Architecture in Java

This repository contains an implementation for a Spring-based application that illustrates the hexagonal architecture in Java.
An article on the topic can be found here :  [Medium](https://medium.com/@anirban99/hexagonal-architecture-in-java-9031d3570d15) | [Blog](https://nomadicguru.in/blog/hexagonal-architecture-in-java/)

## Getting Started

### Requirement

This application requires Java 8 or later.

### Building and running the application

To build the application run this command in the project directory:
```
mvn package
```
To start the application run this command:
```
mvn spring-boot:run
```
The endpoints can be accessed on:
```
http://localhost:8080/
```

### Integration with IntelliJ IDEA

After cloning this repository you can import the project into your IDE using the following steps:
```
File > New > Project from Existing Sources > {Choose directory and Maven as Build Tool}
```

The API specification for this application can be found here : [Open API Specification](./specs/hexagonal-architecture-api.openapi.json)