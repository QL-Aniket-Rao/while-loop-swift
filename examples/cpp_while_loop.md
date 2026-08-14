# C++ While Loop

A while loop in C++ is a fundamental control flow statement used to execute a block of code repeatedly as long as a given boolean condition remains true. Like most languages, the condition is evaluated at the start of each iteration.

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
        // Output the current count
        std::cout << "Current count: " << count << std::endl;
        
        // Increment the counter
        count++; 
    }
    
    std::cout << "While loop finished!" << std::endl;
    return 0;
}
```

## Explanation
1. **Setup**: We include `<iostream>` for input/output operations and define the `main` function.
2. **Initialization**: We declare and initialize `int count = 1;` before the loop.
3. **Condition Check**: The `while (count <= 5)` condition is evaluated. If it's true, the loop body executes.
4. **Execution**: `std::cout` prints the current value of `count` to the console.
5. **Iteration/Update**: `count++;` increments the counter. This step ensures the loop progresses towards its termination condition.
6. **Termination**: Once `count` exceeds 5, the condition becomes false, and the program execution continues after the loop.