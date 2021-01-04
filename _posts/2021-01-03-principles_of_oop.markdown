---
layout: post
title:      "Principles of OOP"
date:       2021-01-04 01:07:29 +0000
permalink:  principles_of_oop
---


Abstraction - The complexities of parts of the program should be hidden from the places they are used. This is "black box" programming. For example, suppose I have a class called "Math" that has many math equations for algebra, geometry, and calculus. If I am using this class in another class called "Car", I want a simple flow of inputing and outputting numbers. I don't need to know the internal complexities of the "Math" class when i'm inside the "Car" class.

Encapsulation - Objects should hide certain attributes. Languages usually use the private, protected, internal, and public keywords to enforce this. For example, some variables are not supposed to be access outside of the class. If there is a need of only one of reading or writing a variable, but not both, then there should be either a getter or a setter method.

Inheritance - Objects can build off on another. For example, if I have a class Shape, I should be able to build two more classes called Square and Circle that have the required features of the Shape class. The Shape class will contain information shared across all types of shapes, such as position, scale, color, name, and more. The individual Square and Circle classes will define variables and methods for only Squares or Circles, respectively. Circles only need to have radius, circumference, and other information relating to circles. Squares, on the other hand, need to know side length.

Polymorphism - The word polymorphism means “many forms.” In programming, this refers to objects taking different names and states. There are two basic types of polymorphism: static and dynamic. Static polymorphism is when a child class overloads a method in it's parent class. This is called static polymorphism because the method that needs to be called can be calculated at runtime. Dynamic polymorphism allows the program to see objects through the lenses of one of its parents. Here is an example of dynamic polymorphism:

```
class Job {
  public void writeName() {
    System.out.println(“Job”);
  }
}

class Firefighter extends Job {
  public void writeName() {
    System.out.println("Firefighter");
  }
}

class Programer extends Job {
  public void writeName() {
    System.out.println("Programmer");
  }
}

class Main {
  public static void main(String[] args) {
    Job myJob = new Job();
    Job myFirefighter = new Firefighter();
    Job myProgrammer = new Programmer();
    myJob.writeName();
    myFirefighter.writeName();
    myProgrammer.writeName();
  }
}
```

The output of the program will be as follows:

```
Job
Firefighter
Programmer
```

Although the myFirefighter object is declared as a Job, it is initialized as a Firefighter. I have access to the Firefighter object through the myFirefighter reference.

Sources:
https://www.w3schools.com/java/java_polymorphism.asp
https://stackify.com/oop-concept-polymorphism/
