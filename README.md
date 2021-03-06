Spring Boot Workshop
----------------------------------------------

This repository show you how to create a basic project using Spring Boot and this topics:

* Building a basic MVC Spring Boot project
* Adding Spring Data JPA
* Model validation with Hibernate Validator
* Adding Thymeleaf
* Adding Bootstrap

#### Create Project

In order to create a basic Spring Boot project you need to install [SDKMAN](http://sdkman.io/) if you are using Linux or Mac, or [posh-gvm](https://github.com/flofreud/posh-gvm) if you are using Windows. After that you can easily install:

* Spring Boot
* Groovy
* Gradle

Then execute this command in your terminal.


```bash
spring init --dependencies=web --language=groovy --build=gradle spring-boot-workshop
```


#### Setup

Create a MySQL database and create an user and password that owns that database, then update the `application.properties` with your credentials

```properties
spring.datasource.url=jdbc:mysql://localhost/springboot_workshop
spring.datasource.username=user
spring.datasource.password=password
spring.datasource.driver-class-name=com.mysql.jdbc.Driver

spring.jpa.generate-ddl=true

spring.messages.basename=i18n/messages
```


#### To Run the Project

```bash
gradle bootRun
```

#### Read this as Reference

* http://josdem.io/techtalk/spring/spring_boot/
* http://josdem.io/techtalk/spring/spring_boot_thymeleaf/
* http://josdem.io/techtalk/spring/spring_boot_internationalization/
* http://josdem.io/techtalk/spring/spring_boot_bower_plugin/
* http://josdem.io/techtalk/spring/spring_boot_validation/
