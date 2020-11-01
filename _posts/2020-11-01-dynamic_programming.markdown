---
layout: post
title:      "Dynamic Programming"
date:       2020-11-01 23:35:42 +0000
permalink:  dynamic_programming
---


"An algorithm is simply a set of steps used to complete a specific task" (Computer Science: Algorithms). Dynamic programming is a technique to solve some types of algorithm problems. Algorithms have many applications in computer science. Therefore, dynamic programming will be a useful tool in the programmer's tool belt in solving problems that pop up in a programmer's career.

Dynamic programming is an optimization over plain recursion. The main principle of dynamic programming is to store some results of the algorithm as the algorithm progresses, so they do not have to be calculated again later. This can greatly reduce time complexities of some solutions. As an example, by using dynamic programming, the Fibonacci Numbers problem can go from exponential time complexity to linear time complexity. (Dynamic Programming) 

```
//Using standard recursion
//Exponential time
int fib(int n)
{
    if (n <= 1)
		    return n;
	  return fib(n-1) + fib(n-2);

}

//Using dynamic programming
//Linear time
int fib_dp(int n)
{
    f[0] = 0;
		f[1] = 1;
		
		for(i = 2; i <= n; i++)
		{
		    f[i] = f[i-1] + f[i-2];
		}
		
    return f[n];
}

```


Luckily, in the example above, the dynamic programming solution is not much more difficult to understand than the recursion solution. It simply stores the values of each fib number in f, instead of calculating it again. Some other problems that can be solved with dynamic programming include ugly numbers, nth Catalan Number, Bell Numbers, Binomial Coefficient, and Permutation Coefficient. Solutions to these problems using Dynamic Programming, in addition to many other types of problems, can be found here: https://www.geeksforgeeks.org/dynamic-programming/ . 

I also believe that programmers can be creative and find ways to solve difficult problems that haven't been discovered yet. When designing the overall structure of code, it may be easier than it sounds to find a treasure that no one else has found before. Another very important use of Dynamic Programming is to pass technical interviews. Even if you may never use it in real life, and if all else fails, there is a chance it will show up in a technical interview and be used in coding challenges. You never know when it may become useful. Try to stretch yourself and use it in ways that are unexpected - but still very powerful. 

References:
Computer Science: Algorithms. https://edu.gcfglobal.org/en/computer-science/algorithms/1/. 

Dynamic Programming. GeeksforGeeks. https://www.geeksforgeeks.org/dynamic-programming/. 
