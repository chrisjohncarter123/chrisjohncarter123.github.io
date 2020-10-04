---
layout: post
title:      "Understanding Time Complexities"
date:       2020-10-04 23:40:04 +0000
permalink:  understanding_time_complexities
---


A fast computer is a happy user. There has been a great growth of understanding of making algorithms that are able to complete their tasks as quickly as possible. Today, computers are able calculate things at blazing speeds. The speed of algorithms can be in both hardware and software. In computer science, time complexities are a way to estimate the speeds of algorithms in the software.

In computing large numbers of data, it is more important for algorithms to be fast in large data sets than in small ones (even though they are both important). 

Some examples of times that an algoithm may take are n^2, n, and log n. Out of these three, log n is the fastest (and best), n is in the middle, and n^2 is the slowest. Some algoithms may end up with the same result, but at different speeds. Here is an example of an algorith taking n^2 time:

```
int n = 10;
for(int i = 0; i < n; i++) {

    for(int j = 0; j < n; j++){
		    console.log( "hello" );
		}

|
```

The code above will print out ``` hello ``` a total of 100 times because ``` n ``` is equal to ``` 10 ```, and there are two loops performed using n ``` n ``` as a counter. This algorithm will take n^2 time.

Here is another algorithm that only takes n time and still prints out ``` hello ``` 100 times:

```
int n = 100;
for(int i = 0; i < n; i++) {

    console.log( "hello" );
		
|
```

Although this example may seem trivial, it is a good example of the importance of using algorithms with low time complexities. Suppose ``` n ``` was 10 million. It would take significantly less time for the seccond algorithm to complete than for the first one.

There are many algorithms for sorting, searching, and selecting elements in different types of data structures. Here is a cheat sheet of time complexities of various algoriths in various senarios: https://www.bigocheatsheet.com/ . I recomend saving this page for future reference, because it can be very useful in finding the best algorithm for specific situations. It also can help in creating new algorithms and solving difficult problems 




**References:**

https://www.geeksforgeeks.org/understanding-time-complexity-simple-examples/

https://www.bigocheatsheet.com/
