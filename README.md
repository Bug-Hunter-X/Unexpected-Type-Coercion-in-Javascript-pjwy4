# Unexpected Type Coercion in Javascript
This repository demonstrates a common but easily overlooked error in JavaScript: unexpected type coercion. The bug arises from the implicit type conversion that occurs when adding a number and a string. This can lead to unexpected results and make debugging more difficult.
## Bug Description
The `foo` function is intended to add two numbers. However, when called with a number and a string, JavaScript coerces the number to a string before performing concatenation instead of addition. 
## Bug Solution
The solution involves explicitly converting the inputs to numbers using `parseInt` or `Number` before performing addition. This ensures that the addition operation works as expected, preventing type coercion issues.
## How to Reproduce
1. Clone the repository.
2. Run `bug.js` using a Node.js environment.
3. Observe the unexpected output (the string "11" instead of the number 2).
4. Run `bugSolution.js` to see the correct implementation and the expected output.