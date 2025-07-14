# API-Gateway

## About
This service represents an API Gateway. Main feature of this service is to accept requests
from clients and route them to the appropriate backend service. It acts as a single entry
point into a system of backend APIs.

## System Requirements

- Java 21
- Apache Maven 3.9.9
- Docker (if running the service within the Docker container)

## How to Install?

### 1. Clone the repository
```shell
git clone https://github.com/Evidentor/API-Gateway.git
cd API-Gateway
```

### 2. Install dependencies
```shell
mvn clean install
```

## How to Run?

### Run with java
```shell
java --enable-preview -jar target/*.jar
```

### Run with docker
#### 1. Build the docker image
```shell
docker build -t api-gateway .
```

#### 2. Create the docker container
```shell
docker run -d --network host --name api-gateway api-gateway:latest
```

#### 3. Stop the docker container
```shell
docker stop api-gateway
```

#### 4. Start the docker container
```shell
docker start api-gateway
```

## How to Test?
```shell
mvn test
```
