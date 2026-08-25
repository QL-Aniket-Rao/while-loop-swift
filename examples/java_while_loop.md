# Java While Loop

A while loop in Java is a control flow statement that allows code to be executed repeatedly as long as a specified boolean condition remains true. It checks the condition *before* executing the loop body. This means that if the condition is initially false, the loop body will never execute.

## Syntax

```java
while (condition) {
    // Code to be executed repeatedly
    // Must include a statement that eventually makes the condition false
}
```

## Example: Counting from 1 to 5

This example demonstrates a basic while loop that prints numbers from 1 to 5.

```java
public class WhileLoopExample {

    public static void main(String[] args) {
        // Initialize the counter variable
        int count = 1;

        System.out.println("Starting the Java While Loop example...");

        // The loop continues as long as 'count' is less than or equal to 5
        while (count <= 5) {
            // Print the current value of count
            System.out.println("Current count: " + count);

            // Increment the counter to move towards the termination condition
            count++; 
        }

        System.out.println("While loop finished. Count is now: " + count);
    }
}
```

### Explanation

1.  **Initialization**: The variable `count` is initialized to 1 outside the loop. This is crucial for starting the count.
2.  **Condition Check**: The `while (count <= 5)` statement is checked before every iteration. If `count` is 5 or less, the code block inside the curly braces executes.
3.  **Execution**: Inside the loop, the current `count` is printed.
4.  **Iteration/Update**: `count++` increments the counter. This step is vital; without it, the condition (`count <= 5`) would always be true, resulting in an infinite loop.
5.  **Termination**: When `count` becomes 6, the condition `(6 <= 5)` evaluates to false, and the loop terminates.