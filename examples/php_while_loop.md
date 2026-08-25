# PHP While Loop

A while loop in PHP is a fundamental control structure that repeatedly executes a block of code as long as a specified boolean condition is true. Like Java, PHP evaluates the condition *before* running the loop body. If the condition is false initially, the loop is skipped entirely.

## Syntax

```php
<?php
while (condition) {
    // Code to be executed repeatedly
    // Must include a statement that eventually makes the condition false
}
?>
```

## Example: Counting from 1 to 5

This example demonstrates a basic while loop in PHP that prints numbers from 1 to 5.

```php
<?php
// Initialize the counter variable
$count = 1;

echo "Starting the PHP While Loop example...<br>";

// The loop continues as long as $count is less than or equal to 5
while ($count <= 5) {
    // Print the current value of $count
    echo "Current count: " . $count . "<br>";

    // Increment the counter to move towards the termination condition
    $count++; 
}

echo "While loop finished. Count is now: " . $count . "<br>";
?>
```

### Explanation

1.  **Initialization**: The variable `$count` is set to 1 before the loop begins.
2.  **Condition Check**: The `while ($count <= 5)` condition is checked at the start of each iteration. If true, the code inside the loop executes.
3.  **Execution**: The current value of `$count` is displayed.
4.  **Iteration/Update**: `$count++` increases the value of `$count`. This update is mandatory to ensure the loop eventually terminates and avoids an infinite loop.
5.  **Termination**: Once `$count` exceeds 5 (i.e., becomes 6), the condition evaluates to false, and the loop stops.