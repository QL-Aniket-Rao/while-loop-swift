# Swift While Loop

A while loop in Swift is a control flow statement that allows a block of code to be executed repeatedly as long as a given Boolean condition remains true. It is similar to loops found in other C-style languages.

## Syntax
```swift
while condition {
    // code to be executed while the condition is true
}
```

## Example
This example demonstrates a simple while loop in Swift that counts from 1 to 5.

```swift
// Initialize the counter variable
var count = 1

print("Starting Swift While Loop...")

// The loop continues as long as 'count' is less than or equal to 5
while count <= 5 {
    print("Current count: \(count)")
    // Increment the counter. This is crucial to prevent an infinite loop.
    count += 1 
}

print("While loop finished!")
```

## Explanation
1. **Initialization**: We declare a mutable variable (`var`) `count = 1`. Swift variables must be mutable if their value is expected to change during the loop.
2. **Condition Check**: The `while count <= 5` statement checks the Boolean condition. If true, the loop body executes.
3. **Execution**: The current value of `count` is printed using string interpolation (`\(count)`).
4. **Iteration/Update**: `count += 1` increments the counter. This step ensures that the condition eventually evaluates to false.
5. **Termination**: Once `count` is 6, the loop condition fails, and the program continues after the loop.