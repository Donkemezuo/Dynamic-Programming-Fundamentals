# Dynamic-Programming-Fundamentals

This playground project provides a fundamental understanding of dynamic programming (DP) as a problem-solving technique.

## What is Dynamic Programming?

Dynamic programming (DP) is an optimization technique used to solve problems by breaking them down into overlapping subproblems and storing previously computed results. It can be seen as an enhanced form of recursion that avoids redundant calculations.

## Difference Between DP and Recursion

A key difference between DP and standard recursion is how states (function arguments) are handled:

1. Recursion: Each state is computed once and never revisited. For example, in depth-first search (DFS), each node is visited only once.
2. Dynamic Programming: States (arguments) may be revisited multiple times, potentially leading to an exponential runtime if not optimized.

## How to Optimize DP to Avoid Exponential Time Complexity?

One key technique to improve efficiency is memoization:

## Memoization
Memoization is a technique where previously computed results are stored and retrieved when needed, rather than recalculating them. This is typically done using a hashmap (dictionary), where; 
1. When a function is called with a specific argument (state), the result is stored in the hashmap after computation.
2. If the same state is encountered again, the stored result is retrieved instantly instead of recomputing it.
3. By using memoization, dynamic programming significantly reduces redundant calculations, making recursive solutions feasible for large inputs.

## The Dynamic Programming Approaches
1. Top-Down approach → is the method of using recursion with memoization for fast computational time. 
It is a top down approach because we start from the top and recursively move down towards the base case.

2. Bottom-Up approach → on the contrast, the Bottom-Up method starts from the base case and works up to the larger problem.

## Top-Down vs Bottom-Up 
Bottom-Up approach is faster since iteration has less overhead than recursion.
The Top-Down approach is easier to write.

## When to use Dynamic Programming technique for problem solving? 
1. When the problem is asking for the optimal value (max or min) of something or the number of ways to do something. Questions like;
    a). What is the minimum cost of doing something?
    b). What is the maximum profit of X?
    c). How many ways are there to do Y?
    d). What is the longest possible ABC?
    
2. Problems where at each step, there is a decision to make and such decisions affect future decisions.
    a). A decision could be picking between two elements 
    b). Decisions affecting future decisions could be something like “if you take an element X, then you can’t take an element Y in the future.” This idea is what separates Dynamic programming with Greedy. With greedy technique, local decisions do not affect other decisions. 

## The Schematics of solving Dynamic Programming Questions
To create any DP algorithm, there are 3 main components;
1. A data structure to compute or hold the answer to the problem at any given state. I.e a key-value pair data structure where each key is the state and each value of that key is the answer to the problem in that state. OR a function that given a state as input, can compute the answer to the problem at that state or input. 
2. A recurrence relation to transition between states. 


