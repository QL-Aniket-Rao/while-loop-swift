# Swift While Loop

A while loop in Swift is a fundamental control flow structure that repeatedly executes a block of code as long as a specified boolean condition evaluates to `true`. It is ideal when the number of iterations is not known beforehand.

## Syntax
```swift
while condition {
    // code to be executed while the condition is true
}
```

## Example
This example demonstrates a simple while loop that counts from 1 to 5.

```swift
var count = 1
print("Starting Swift While Loop...")

// The loop continues as long as 'count' is less than or equal to 5
while count <= 5 {
    print("Current count: \(count)")
    // Increment the counter to eventually make the condition false
    count += 1
}

print("While loop finished!")
```

## Explanation
1. **Initialization**: We declare and initialize `var count = 1`. The `var` keyword allows the value to be mutable (changeable).
2. **Condition Check**: `while count <= 5` checks the condition before each iteration. If `count` is 5 or less, the loop body executes.
3. **Execution**: Inside the loop, the current value of `count` is printed using string interpolation `\(count)`.
4. **Iteration/Update**: `count += 1` (which is shorthand for `count = count + 1`) increments the counter. This step is necessary to prevent an infinite loop.
5. **Termination**: Once `count` becomes 6, the condition `6 <= 5` evaluates to `false`, and the loop exits.