# NewsTok API Gateway

Welcome to the NewsTok API Gateway repository! This repository contains the components needed for routing requests between microservices and handling service discovery.

## Overview

The NewsTok API Gateway includes:

1. **Eureka Server**: Handles service discovery for microservices.
2. **API Gateway**: Routes incoming requests to the appropriate backend services.

## Prerequisites

Before running the application, ensure you have the following:

- **Java 11 or later**: Required for running the Spring Boot applications.
- **Maven**: For building the Java projects.

## Setup Instructions

### 1. Clone the Repository

First, clone the repository into your local environment:

```bash
# Clone the repository
git clone https://github.com/PaleBlueDot-repo/newstok-Api-Gateway.git

# Navigate into the cloned directory
cd newstok-Api-Gateway
```

### 2. Run the Eureka Server

1. Navigate to the `Eureka-Server` directory:

   ```bash
   cd Eureka-Server
   ```

2. Build and run the Eureka Server using Maven:

   ```bash
   mvn spring-boot:run
   ```

   The Eureka Server will start and be available at `http://localhost:8761`.

### 3. Run the API Gateway

1. After the Eureka Server is running, navigate to the `ApiGateway` directory:

   ```bash
   cd ../ApiGateway
   ```

2. Build and run the API Gateway using Maven:

   ```bash
   mvn spring-boot:run
   ```

   The API Gateway will start and be available at `http://localhost:8080`.

## Accessing the Application

- **Eureka Server**: Visit `http://localhost:8761` to view the Eureka dashboard and see registered microservices.
- **API Gateway**: Visit `http://localhost:8080` to interact with the API Gateway.

