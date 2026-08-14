# PHP While Loop

A while loop in PHP is a control structure that repeatedly executes a block of code as long as a specified condition evaluates to true. Like in other languages, the condition is checked at the beginning of the loop iteration.

## Syntax
```php
while (condition) {
    // code to be executed while the condition is true
}
```

## Example
This example demonstrates a basic while loop in PHP that counts from 1 to 5.

```php
<?php
// Initialize the counter variable
$count = 1;

echo "Starting PHP While Loop...<br>";

// The loop continues as long as $count is less than or equal to 5
while ($count <= 5) {
    // Output the current count
    echo "Current count: " . $count . "<br>";
    
    // Increment the counter
    $count++; 
}

echo "While loop finished!<";
?>
```

## Explanation
1. **Initialization**: We initialize the variable `$count = 1;` before the loop starts.
2. **Condition Check**: The `while ($count <= 5)` statement checks the condition. If true, the code block inside the loop executes.
3. **Execution**: The current value of `$count` is echoed (printed).
4. **Iteration/Update**: `$count++` increases the value of `$count`. This ensures that the loop eventually reaches a state where the condition is false.
5. **Termination**: When `$count` becomes 6, the condition fails, and the program exits the loop.