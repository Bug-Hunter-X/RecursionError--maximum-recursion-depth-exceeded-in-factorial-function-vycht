# RecursionError in Factorial Function

This repository demonstrates a common error in recursive functions: exceeding the maximum recursion depth.  The `factorial.py` file contains a factorial function that works for non-negative inputs but throws a `RecursionError` when a negative number is provided. The `factorialSolution.py` provides a corrected version.

**How to reproduce:**

1. Clone this repository.
2. Run `bug.py`.
3. Observe the `RecursionError` when calling `factorial()` with a negative argument.
4. Run `bugSolution.py` to see the corrected implementation.

**Explanation:**

Recursive functions require a base case to stop the recursion. The original factorial function only handles the base case of n=0. Providing a negative number leads to infinite recursion, causing a stack overflow.