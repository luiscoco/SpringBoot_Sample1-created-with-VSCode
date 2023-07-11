# SpringBoot_Sample1-created-with-VSCode

Create a SpringBoot project with VSCode
![Create a SpringBoot project with VSCode](https://github.com/luiscoco/SpringBoot_Sample1-created-with-VSCode/assets/32194879/39b155f8-0c2d-4e43-9154-59ff7f39f0ee)

Select the Maven project type
![Select the Maven project type](https://github.com/luiscoco/SpringBoot_Sample1-created-with-VSCode/assets/32194879/c5b709a9-1903-4e87-a5de-8e6b414a9098)

Select the SpringBoot version
![Select the SpringBoot version](https://github.com/luiscoco/SpringBoot_Sample1-created-with-VSCode/assets/32194879/85ab5aa6-a5d2-443d-aa31-ba93adb004eb)

Select the project language Java
![Select the project language Java](https://github.com/luiscoco/SpringBoot_Sample1-created-with-VSCode/assets/32194879/3872bf2b-62e2-4d60-b991-015357d3c8f6)

Input Group Id for your project
![Input Group Id for your project](https://github.com/luiscoco/SpringBoot_Sample1-created-with-VSCode/assets/32194879/12ea1d5f-982d-46bc-a4f5-174a133b0aca)

Input Artifact Id for your project
![Input Artifact Id for your project](https://github.com/luiscoco/SpringBoot_Sample1-created-with-VSCode/assets/32194879/3a6d675c-0139-4cd4-b260-e823b6ee1657)

Specify packaging type
![Specify packaging type](https://github.com/luiscoco/SpringBoot_Sample1-created-with-VSCode/assets/32194879/7c49d8c2-8b32-4e3e-addd-593d76538691)

Specify the Java version
![Specify the Java version](https://github.com/luiscoco/SpringBoot_Sample1-created-with-VSCode/assets/32194879/d27229a4-05ba-4ea5-9fea-777193bacd3a)

Search for dependencies
![Search for dependencies](https://github.com/luiscoco/SpringBoot_Sample1-created-with-VSCode/assets/32194879/db8baab0-b02c-492e-bd02-7679ce5c0d69)

Select the project folder
![Select the project folder](https://github.com/luiscoco/SpringBoot_Sample1-created-with-VSCode/assets/32194879/065d0289-0ee5-4945-80d5-f83058cba253)

Open the SpringBoot project
![Open the SpringBoot project](https://github.com/luiscoco/SpringBoot_Sample1-created-with-VSCode/assets/32194879/0d4c87ef-1dd4-4291-b9fc-4debdd5ae66d)

SpringBoot project structure and default code
![SpringBoot project structure and default code](https://github.com/luiscoco/SpringBoot_Sample1-created-with-VSCode/assets/32194879/4b52e179-c0dd-48d8-8190-c37ab0c60678)

pom_xml file
![pom_xml file](https://github.com/luiscoco/SpringBoot_Sample1-created-with-VSCode/assets/32194879/f046845b-cf69-4201-abc6-638510460bfa)

To create the Github repository
![To create the Github repository](https://github.com/luiscoco/SpringBoot_Sample1-created-with-VSCode/assets/32194879/179edb08-6e93-425a-ada4-996cf62d9a17)

Set Github repository name and public repo
![Set Github repository name and public repo](https://github.com/luiscoco/SpringBoot_Sample1-created-with-VSCode/assets/32194879/8c95a3c8-6d54-4ab6-917b-256fc5773a7a)

Open the Github repository
![Open the Github repository](https://github.com/luiscoco/SpringBoot_Sample1-created-with-VSCode/assets/32194879/b81929ee-b75c-4dd7-863d-2759cb16bc68)

## Following steps
Set the running port in the application_properties file
![Set the running port in the application_properties file](https://github.com/luiscoco/SpringBoot_Sample1-created-with-VSCode/assets/32194879/9c084e5f-efa0-44ce-9922-db5c6f3e0407)

pom_xml modifications added
![pom_xml modifications added](https://github.com/luiscoco/SpringBoot_Sample1-created-with-VSCode/assets/32194879/a8e51217-2aff-49d7-afea-95dda7fa8d5f)

To install maven run the command:
```
mvn clean install
```

To run the project type the command:
```
mvn spring-boot:run
```
or 
```
mvn spring-boot:run -Dspring-boot.run.arguments=--server.port=8080
```

We also added a "Hello World" message in the code:
```java
package com.example.demo;

import org.springframework.boot.SpringApplication;
import org.springframework.boot.autoconfigure.SpringBootApplication;

@SpringBootApplication
public class DemoApplication {

    public static void main(String[] args) {
        SpringApplication.run(DemoApplication.class, args);
        System.out.println("Hello World");
    }

}
```

Also you can set the running port in the pom.xml file:

POM.xml Configuration:
Alternatively, you can configure the server.port property directly in your project's pom.xml file. Add the following configuration within the <build> section:
```xml
<plugins>
    <plugin>
        <groupId>org.springframework.boot</groupId>
        <artifactId>spring-boot-maven-plugin</artifactId>
        <configuration>
            <arguments>
                <argument>--server.port=8080</argument>
            </arguments>
        </configuration>
    </plugin>
</plugins>
```














