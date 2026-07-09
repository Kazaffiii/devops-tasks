# DevOps Tasks

This repository contains my hands-on DevOps labs and practice projects.

## Repository Structure

```
devops-tasks/
├── gradle-lab/
│   ├── build.gradle
│   ├── settings.gradle
│   └── src/
├── maven-lab/
│   ├── pom.xml
│   └── src/
└── README.md
```

## Labs

### Lab 1 - Building and Packaging Java Application with Gradle
- Install Gradle
- Clone Java application
- Run unit tests
- Build the application
- Generate build/libs/calculator.jar
- Run and verify the application

### Lab 2 - Building and Packaging Java Application with Maven
- Install Maven
- Clone Java application
- Run unit tests
- Build the application
- Generate target/calculator.jar
- Run and verify the application
# Docker Lab 3 - Spring Boot Application

## Overview

This project demonstrates how to containerize a Java Spring Boot application using Docker and Maven.

## Technologies Used

- Java 17
- Spring Boot
- Maven
- Docker

## Project Structure

```
Docker-1/
├── src/
├── target/
├── pom.xml
├── Dockerfile
└── README.md
```

## Dockerfile

The Dockerfile performs the following steps:

1. Uses the Maven image with Eclipse Temurin Java 17.
2. Creates a working directory.
3. Copies the application source code.
4. Builds the project using Maven.
5. Exposes port 8080.
6. Runs the generated JAR file.

## Build Docker Image

```bash
docker build -t app1 .
```

## Verify Image

```bash
docker images
```

## Run Container

```bash
docker run -d --name container1 -p 8080:8080 app1
```

## Test the Application

Open your browser:

```
http://localhost:8080
```

or use:

```bash
curl http://localhost:8080
```

## Stop Container

```bash
docker stop container1
```

## Remove Container

```bash
docker rm container1
```

## Technologies

- Java 17
- Git & GitHub
- Gradle
- Maven

## Author

Ahmed Elkazafi

GitHub: https://github.com/Kazaffiii
