# C++ While Loop

A while loop in C++ is a fundamental looping construct that repeatedly executes a block of code as long as a specified Boolean condition remains true. Like Java and Swift, it checks the condition before each iteration.

## Syntax
```cpp
while (condition) {
    // code to be executed while the condition is true
}
```

## Example
This example demonstrates a basic while loop in C++ that counts from 1 to 5.

```cpp
#include <iostream>

int main() {
    // Initialize the counter variable
    int count = 1;

    std::cout << "Starting C++ While Loop..." << std::endl;

    // The loop continues as long as 'count' is less than or equal to 5
    while (count <= 5) {
        // Print the current count
        std::cout << "Current count: " << count << std::endl;
        
        // Increment the counter
        count++; 
    }
    
    std::cout << "While loop finished!" << std::endl;
    return 0;
}
```

## Explanation
1. **Initialization**: We declare and initialize an integer variable `int count = 1;`.
2. **Condition Check**: The `while (count <= 5)` statement evaluates the condition. If true, the loop body is executed.
3. **Execution**: `std::cout` is used to print the current value of `count` to the console.
4. **Iteration/Update**: `count++;` increments the counter. This essential step prevents an infinite loop by ensuring the condition eventually becomes false.
5. **Termination**: When `count` becomes 6, the condition fails, and the program execution moves past the loop.