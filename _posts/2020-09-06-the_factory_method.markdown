---
layout: post
title:      "The Factory Method"
date:       2020-09-07 03:48:11 +0000
permalink:  the_factory_method
---



In this post, I want to talk about the factory method.

The factory method is a design pattern that organizes the way subclasses are created. Design patterns such as the factory method are great at making code more readable by other programmers. When programmers look at code, it takes some precious brain power to understand it. A programmer only has so much brain power a day to use at work before it needs to recharge. Using programing patterns, the programmer can quickly relate to new code by seeing patterns he/she already knows well. Instead of carefully going line-by-line, method-by-method, the programmer can take a quick look and think "Ah, I see a factory method pattern is used here" 

Here is a quick definition of the factory method: "Factory Method is a creational design pattern that provides an interface for creating objects in a superclass, but allows subclasses to alter the type of objects that will be created." (Factory Method)

The factory method is a way to create new objects. The initialization logic is placed in a factory method instead of the object constructor. Also, "Objects returned by a factory method are often referred to as products." (Factory Method) However, many times the factory method can make code more complicated because of the addition of new subclasses.

The key benefit of this pattern is that child objects can change the initialization code of new objects. This is a very common problem because inheritance is a vital component of many programming languages. Therefore, this programming pattern may prove to be worth learning and using frequently. 








**References**:

Factory Method. (n.d.). Retrieved September 07, 2020, from https://refactoring.guru/design-patterns/factory-method
