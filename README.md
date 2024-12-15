# PHP Function Unexpected Behavior with Zero Arguments

This repository demonstrates a subtle bug in a simple PHP function that exhibits unexpected behavior when both input arguments are zero. The function `my_function` aims to add two numbers, but its handling of the edge case where both arguments are zero results in incorrect output. 

## Bug Description
The function `my_function` uses a strict equality check (`===`) to check if the first argument is zero. While this works correctly for cases where one argument is zero and the other is not, the result is unexpectedly zero when both arguments are zero. The intended behavior would be to return zero in such case. However, it currently returns zero due to the logic.

## Solution
The solution involves modifying the conditional statement to explicitly handle the case where both arguments are zero. This ensures that the function behaves as expected in all scenarios.