# C++ While Loop

A while loop in C++ is a looping construct that executes a block of code repeatedly as long as a specified boolean expression evaluates to true. It is a pre-test loop, meaning the condition is checked before the body of the loop runs.

## Syntax
```cpp
while (condition) {
    // code to be executed while the condition is true
}
```

## Example
This example demonstrates a simple while loop that counts from 1 to 5.

```cpp
#include <iostream>

int main() {
    // Initialize the counter variable
    int count = 1;

    std::cout << "Starting C++ While Loop..." << std::endl;

    // The loop continues as long as 'count' is less than or equal to 5
    while (count <= 5) {
        std::cout << "Current count: " << count << std::endl;
        // Increment the counter to eventually make the condition false
        count++; 
    }
    
    std::cout << "While loop finished!" << std::endl;
    return 0;
}
```

## Explanation
1. **Initialization**: We declare and initialize `int count = 1;` outside the loop to set the starting point.
2. **Condition Check**: The `while (count <= 5)` statement is checked before every iteration. If the condition is true, the loop body executes.
3. **Execution**: Inside the loop, `std::cout` prints the current value of `count` to the console.
4. **Iteration/Update**: `count++;` increments the counter. This is critical to ensure the loop eventually terminates.
5. **Termination**: When `count` becomes 6, the condition `6 <= 5` evaluates to false, and the program proceeds past the loop.