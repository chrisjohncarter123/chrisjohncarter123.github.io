---
layout: post
title:      "Angular Overview "
date:       2020-09-20 21:53:57 +0000
permalink:  angular_overview
---


Angular is one of the most popular front end frameworks developed by google.

> "Angular is an application design framework and development platform for creating efficient and sophisticated single-page apps." (https://angular.io/docs)
> 


Angular makes it easy to develop applications across all different platforms including web, mobile web, native mobile and native desktop. It uses the maximum speed possible and gives control over scalability. It provides features for huge data requirements by building data models on RxJS, Immutable.js, or other push-models.

Angular has a very large following, well into the millions.There are many pluigins for IDEs that give all the standard tools expected for any large framework. It has a good doccumentation, making it easy to learn and troubleshoot problems. There are also numerous online classes and videos to make getting up and running fairly easy. 

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

I reccomend developing angular in WebStorm by JetBrains. It is a JavaScript IDE that is known for having a lot of features like InteliJ. 





