---
layout: post
title:      "Introduction to Java Spring"
date:       2020-10-11 08:19:13 +0000
permalink:  introduction_to_java_spring
---


Spring is a very popular Java framework used to develop websites. In fact, it is one the most popular Java frameworks in the world. According to the Spring website, "Spring makes programming Java quicker, easier, and safer for everybody. Spring’s focus on speed, simplicity, and productivity has made it the world's most popular Java framework."

There are plenty of great tutorials for getting started with Spring on various websites. Almost any website with content for learning will have material for spring including YouTube, Coursea, Udemy, and more. However, I prefer the official Spring tutorials at https://spring.io/quickstart because they are very trustworthy, consice, and practical. They are straight to the point, while other learning platforms give more of a cover-to-cover learning.

Here is a snippet from the first tutorial on the official docs:

```
package com.example.demo;

import org.springframework.boot.SpringApplication;
import org.springframework.boot.autoconfigure.SpringBootApplication;
import org.springframework.web.bind.annotation.GetMapping;
import org.springframework.web.bind.annotation.RequestParam;
import org.springframework.web.bind.annotation.RestController;

@SpringBootApplication
@RestController
public class DemoApplication {

public static void main(String[] args) {
SpringApplication.run(DemoApplication.class, args);
}

@GetMapping("/hello")
public String hello(@RequestParam(value = "name", defaultValue = "World") String name) {
return String.format("Hello %s!", name);
}
}
```

As you can see, Spring makes heavy use of Java annotations. After creating a new Spring project using start.spring.io and adding the above code, the project will be a very simple working Spring application! This is the very beggning, there are countless features of Spring to explore and learn. Don't be fooled - just because you made your first Spring application, that doesn't mean you are an expert yet! Spring uses a long list of technologies including Spring Data, Spring Cloud, Spring Cloud Data Flow, Spring Security, Spring Session, Spring Integration, Spring HATEOAS, Spring Batch, and Spring for Android. An experienced Spring developer will understand the ins and outs of all of these. Each one of these mentioned technologies also has many parts to learn too!

Another close option to spring is ASP.NET core. ASP.NET core uses C# instead of Java. They both have their own strengths and weaknesses, and any project should choose wisley of which one to use. These two options are some of the most popular frameworks for web development. They have been compared many times, and there is a lot of information on the web about when to use which one. 

Here is the official Spring github page: https://github.com/spring-projects/spring-framework/wiki/Spring-Framework-Versions

Sources:

https://spring.io/

https://stackoverflow.com/questions/1408901/asp-net-mvc-vs-spring-mvc
