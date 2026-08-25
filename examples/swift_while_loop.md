# Swift While Loop

A while loop in Swift is a control flow structure that repeatedly executes a block of code as long as a specified Boolean condition remains true. Similar to other languages, Swift checks the condition *before* executing the loop body. If the condition is false at the start, the loop body is never run.

## Syntax

```swift
while condition {
    // Code to be executed repeatedly
    // Must include a statement that eventually makes the condition false
}
```

## Example: Counting from 1 to 5

This example demonstrates a basic while loop in Swift that prints numbers from 1 to 5.

```swift
// Initialize the counter variable
var count = 1

print("Starting the Swift While Loop example...")

// The loop continues as long as 'count' is less than or equal to 5
while count <= 5 {
    // Print the current value of count
    print("Current count: \(count)")

    // Increment the counter to move towards the termination condition
    count += 1
}

print("While loop finished. Count is now: \(count)")
```

### Explanation

1.  **Initialization**: The variable `count` is declared and initialized to 1 using `var` (since it will be modified).
2.  **Condition Check**: The `while count <= 5` statement is evaluated at the start of each iteration. If the condition is true, the code block inside the loop executes.
3.  **Execution**: The current value of `count` is printed using string interpolation (`\(count)`).
4.  **Iteration/Update**: `count += 1` increases the value of `count`. This step is essential to ensure that the condition eventually becomes false, preventing an infinite loop.
5.  **Termination**: When `count` reaches 6, the condition `6 <= 5` becomes false, and the loop terminates.