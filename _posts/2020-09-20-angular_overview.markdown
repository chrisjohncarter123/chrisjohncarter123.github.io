---
layout: post
title:      "Angular Overview "
date:       2020-09-20 17:53:58 -0400
permalink:  angular_overview
---


Angular is one of the most popular front end frameworks developed by google.
> "Angular is an application design framework and development platform for creating efficient and sophisticated single-page apps." (https://angular.io/docs)
> 
Angular makes it easy to develop applications across all different platforms including web, mobile web, native mobile and native desktop. It uses the maximum speed possible and gives control over scalability. It provides features for huge data requirements by building data models on RxJS, Immutable.js, or other push-models. The two other alternatives to Angular are React and Vue. Each framework has their own strengths, weaknesses, communities, and plug-ins, so it is best to research which framework is best for each individual project. 

Angular has a very large following, well into the millions.There are many pluigins for IDEs that give all the standard tools expected for any large framework. It has a good doccumentation, making it easy to learn and troubleshoot problems. There are also numerous online classes and videos to make getting up and running fairly easy. I reccomend developing angular in WebStorm by JetBrains. It is a JavaScript IDE that is known for having a lot of features like InteliJ. It is also an option to use [stackblitz](https://stackblitz.com/angular/vmgxnnvnjyr?file=src%2Fapp%2Fapp.component.ts) as an IDE. It is good for playing around and learning simple concepts with, but for serious learners, a desktop IDE will be requried. 

Here are a simple code snippet taken from the docs:


```
<h2>Products</h2>

<div *ngFor="let product of products">

  <h3>
    <a [title]="product.name + ' details'">
      {{ product.name }}
    </a>
  </h3>

  <p *ngIf="product.description">
    Description: {{ product.description }}
  </p>

  <button (click)="share()">
    Share
  </button>

</div>

```

I think angular is easy to understand if you already know javascript and html. A lot of the code here is easy to guess correctly what it does: ``` *ngfor ``` is a for loop, ``` *ngif ``` is a if statement, and ```  <button (click)="share()"> ``` is a button that calls the ``` share() ``` method when it is clicked.

**Components**

According to the docs, "Components define areas of responsibility in the user interface, or UI, that let you reuse sets of UI functionality. " Therefore, components are very important for organizing and reusing code. Components have a specific purpose that they accomplish in the app. Components have three elements: a component class, an HTML template, and component-specific styles. Angular applications are made out of trees of components. Each of these three elements can take their own file. Usually, each file has the same name with different extenstions. The component class has the .component.ts extention, the html template has the .component.html extention, and the style has the .component.css extention. 

**Sources**:

https://angular.io/start





