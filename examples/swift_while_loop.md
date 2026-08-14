# Swift While Loop

A while loop in Swift executes a block of code repeatedly as long as a specified boolean condition remains true. It is an indefinite loop, meaning it continues until the condition explicitly becomes false.

## Syntax
```swift
while condition {
    // code to be executed while the condition is true
}
```

## Example
This example demonstrates a simple while loop in Swift that counts from 1 to 5.

```swift
var count = 1

print("Starting Swift While Loop...")

// The loop continues as long as count is less than or equal to 5
while count <= 5 {
    print("Current count: \(count)")
    // Increment the counter
    count += 1 
}

print("While loop finished!")
```

## Explanation
1. **Initialization**: We declare and initialize a mutable variable `var count = 1` outside the loop.
2. **Condition Check**: The `while count <= 5` statement checks the condition. If true, the loop body executes.
3. **Execution**: Inside the loop, the current value of `count` is printed.
4. **Iteration/Update**: `count += 1` (which is equivalent to `count = count + 1`) increments the counter. This update is mandatory to prevent an infinite loop.
5. **Termination**: When `count` reaches 6, the condition becomes false, and the loop naturally terminates.