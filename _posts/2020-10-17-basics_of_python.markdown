---
layout: post
title:      "Basics of Python"
date:       2020-10-17 05:45:05 +0000
permalink:  basics_of_python
---



Python is one of the most popular programming languages in the world. it is free and easy to learn. According to the docs, it has efficient high-level data structures and a simple approach to oject-oriented programming. It has elegant syntax and dynamic typing. I has many advantages of different languages. 

Python, like many other languages, has if statements. Here is a simple if statement written in python:

```
myNum = 1
if myNum = 0
    print ("myNum is 0.")
print ("Finished program.")
```

This block of code will test the value of ```myNum```. If it is equal exactly to 0, then the console will print out the string ```"myNum is 0."```. However, the program will always print out ```Finished program.```, and will never acutally print out ```"myNum is 0."```, because the value of ```myNum``` will only ever be 1.

Python also uses for loops, like many other programming languages. The syntax for for loops is very simple, as seen in the example below:

```
list = ['cat', 'dog', 'bird']


for i in range(len(list))
  print(list[i])
```

If you are familiar with for loops from other languages, this is simple enough to understand. However, if you are not familiar with for loops, let me explain about for loops:

Suppose you wanted the code to complete an action a set number of times. You could, for example, copy and paste the same line of code over and over again to acheive the disired result. However, this is very inefficient. What if you wanted to excecute the same code 10000 times? You would have to copy and paste the 10000 times! There is a better solution: loops.

In the for loop above. the code ```print(list[i])``` is repeated for each element in the list. In this case, it is repeated three times because there are three elements in the list. The variable ```i``` is the counter of the current iteration of the loop.It starts at ```0``` and goes to ```2```. It references to correct element in the list each time the ```print``` function is called.

Sources
https://www.python.org/doc/
https://www.programiz.com/python-programming/for-loop

