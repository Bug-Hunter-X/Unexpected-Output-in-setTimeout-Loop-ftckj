# Unexpected Output in setTimeout Loop

This repository demonstrates a common JavaScript error related to closures and the `setTimeout` function within loops.

The `bug.js` file contains code that exhibits the problem. The `bugSolution.js` file provides a corrected version.

## Problem

The expected output would be numbers from 0 to 9 printed sequentially after a one second delay each. However, due to how closures work in JavaScript, the loop finishes and only the final value of 'i' (10) is printed ten times.

## Solution

To fix this, create a closure that captures a copy of the loop variable 'i' in each iteration, preventing the issue.

## How to run

1. Clone the repository.
2. Run `node bug.js` and `node bugSolution.js` in your terminal to see the different outputs.