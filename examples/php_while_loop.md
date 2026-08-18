# PHP While Loop

A while loop in PHP is used to execute a block of code repeatedly as long as a specified condition is true. Like in Java, the condition is evaluated at the beginning of each iteration.

## Syntax
```php
while (condition) {
    // code to be executed while the condition is true
}
```

## Example
This example demonstrates a simple while loop that counts from 1 to 5.

```php
<?php
// Initialize the counter variable
$count = 1;

echo "Starting PHP While Loop...<br>";

// The loop continues as long as $count is less than or equal to 5
while ($count <= 5) {
    echo "Current count: $count<br>";
    // Increment the counter to eventually make the condition false
    $count++; 
}

echo "While loop finished!";
?>
```

## Explanation
1. **Initialization**: We initialize `$count = 1;` to set the starting value for our loop control variable.
2. **Condition Check**: The `while ($count <= 5)` statement checks the condition. As long as this is true, the code inside the loop runs.
3. **Execution**: Inside the loop, the current value of `$count` is printed to the output.
4. **Iteration/Update**: `$count++;` increments the counter. This ensures that the condition eventually becomes false.
5. **Termination**: When `$count` reaches 6, the condition fails, and the loop stops, allowing the script to finish execution.