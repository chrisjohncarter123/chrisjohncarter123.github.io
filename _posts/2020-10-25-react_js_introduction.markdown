---
layout: post
title:      "React.js Introduction"
date:       2020-10-25 08:56:02 +0000
permalink:  react_js_introduction
---


React.js is a front-end framework by Facebook for JavaScript to build SPAs. It is one of the most popular front-end frameworks, used by many large companies. Files have the jsx extension. If you are unfamiliar with the jsx extension, it is like a combination of JavaScript with HTML. They work just like regular JavaScript files, except HTML code snippets can be expressed directly without using quotes. Without jsx, writing files can quickly become very time consuming and confusing. 

Here is an example of a line of code in a JSX file (take from the docs):

```const element = <h1>Hello, world!</h1>;```

Notice this line of code isn't completely JavaScript, nor is it completely HTML. How can this be?! Thankfully, ingenious engineers have designed a perfect solution to the fiasco of this:

```cost element = "<h1>Hello, world!</h1>"```

To the untrained eye, these two lines of code are identical. But the experienced programmer will sigh in frustration at the second line, but be encouraged by the first line. What is the big deal? First of all, nobody wants to go through thousands of lines of code, looking for errors, only to find a misplaced quote. Also, it is a hassle to install all the plugins to color-code the code in an IDE. Please, as an experienced programmer, I ask you to never use the following code:

```cost element = "<h1>Hello, world!</h1>"```

One of the most important features of react.js are components. Components render different parts of the website. Each component has either a function called "render", or the entire component is just a function called "render". This function is where the magic happens - it returns the HTML that is displayed on the webpage. 

Now, components can contain other components, and can take arguments from parent components. Components are used in similar ways that classes are used in other object oriented languages such as C# or Java. It is therefore very important to make components reusable and concise, otherwise the project will quickly become too large and complicated.

Thank you for your time.

Source: https://reactjs.org/docs/introducing-jsx.html

