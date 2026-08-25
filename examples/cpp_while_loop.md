# C++ While Loop

A while loop in C++ is a loop structure that repeatedly executes a block of code as long as a specified Boolean condition evaluates to true. C++ checks the condition *before* entering the loop body. If the condition is false initially, the loop body is never executed.

## Syntax

```cpp
while (condition) {
    // Code to be executed repeatedly
    // Must include a statement that eventually makes the condition false
}
```

## Example: Counting from 1 to 5

This example demonstrates a basic while loop in C++ that prints numbers from 1 to 5.

```cpp
#include <iostream>

int main() {
    // Initialize the counter variable
    int count = 1;

    std::cout << "Starting the C++ While Loop example..." << std::endl;

    // The loop continues as long as 'count' is less than or equal to 5
    while (count <= 5) {
        // Print the current value of count
        std::cout << "Current count: " << count << std::endl;

        // Increment the counter to move towards the termination condition
        count++; 
    }

    std::cout << "While loop finished. Count is now: " << count << std::endl;
    return 0;
}
```

### Explanation

1.  **Initialization**: The integer variable `count` is initialized to 1 before the loop starts.
2.  **Condition Check**: The `while (count <= 5)` statement is evaluated before each iteration. If true, the body of the loop executes.
3.  **Execution**: Inside the loop, the current value of `count` is printed to the console.
4.  **Iteration/Update**: `count++` increments the counter. This is critical for making progress and ensuring the loop eventually stops.
5.  **Termination**: When `count` becomes 6, the condition `(6 <= 5)` evaluates to false, and the program moves past the loop.