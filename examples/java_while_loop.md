# Java While Loop

A while loop in Java is a control flow statement that allows code to be executed repeatedly as long as a specified boolean condition remains true. It checks the condition *before* executing the loop body, meaning the loop might not execute even once if the condition is initially false.

## Syntax
```java
while (condition) {
    // code to be executed while the condition is true
}
```

## Example
This example demonstrates a simple while loop that counts from 1 to 5.

```java
public class WhileLoopExample {
    public static void main(String[] args) {
        // Initialize the counter variable
        int count = 1;

        System.out.println("Starting Java While Loop...");

        // The loop continues as long as 'count' is less than or equal to 5
        while (count <= 5) {
            System.out.println("Current count: " + count);
            // Increment the counter to eventually make the condition false
            count++; 
        }
        
        System.out.println("While loop finished!");
    }
}
```

## Explanation
1. **Initialization**: We start with `int count = 1;`. This sets up the variable we will use for counting.
2. **Condition Check**: The `while (count <= 5)` statement checks if the condition is met. If `count` is 1, 2, 3, 4, or 5, the condition is true, and the loop body executes.
3. **Execution**: Inside the loop, the current count is printed.
4. **Iteration/Update**: `count++` increments the counter. This step is crucial; without it, the condition would always remain true, leading to an infinite loop.
5. **Termination**: Once `count` becomes 6, the condition `count <= 5` evaluates to false, and the loop terminates, allowing the program to proceed to the final print statement.