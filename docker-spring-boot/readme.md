## What is it?
This source code is an Spring Boot web application (mvc + thymeleaf).
 
Tested with
* Docker 19.03
* Ubuntu 19
* Java 8 or Java 11
* Spring Boot 2.2.4.RELEASE
* Maven

For explanation, please visit this article - [Docker and Spring Boot](https://mkyong.com/docker/docker-spring-boot-examples/)

## How to run this?
```bash
$ git clone https://github.com/mkyong/docker-java
$ cd docker-spring-boot
$ mvn clean package
$ java -jar target/spring-boot-web.jar

  access http://localhost:8080

```
## Dockerize & Use

- Create a docker image: `docker build -t bb8docker/spring-boot-hello:1.0 .`
- Push to docker hub: `docker push bb8docker/spring-boot-hello:1.0` 
- Run it locally: `docker run --rm -d -p 8080:8080 -t bb8docker/spring-boot-hello:1.0`
- Access: 
  - http://localhost:8080/
  - http://localhost:8080/test
  - http://localhost:8080/hello
