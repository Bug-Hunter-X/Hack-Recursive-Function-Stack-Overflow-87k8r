# Hack Recursive Function Stack Overflow

This repository demonstrates a common error in Hack: a stack overflow caused by unbounded recursion in a factorial function.

The `bug.hack` file contains the problematic code. The `bugSolution.hack` file provides a solution using iteration to avoid stack overflow.

## Bug Description
The `foo` function calculates the factorial of a number recursively. However, if the input is too large, the recursive calls will exceed the available stack space, resulting in a stack overflow error.

## Solution
The solution replaces the recursive approach with an iterative one using a loop. This prevents stack overflow, even with large input values.

## How to Reproduce
1. Clone this repository.
2. Compile and run `bug.hack` with a large input (e.g., `foo(10000)`).  You will observe a stack overflow.
3. Compile and run `bugSolution.hack` with the same large input. This will execute without a stack overflow and print the correct factorial.