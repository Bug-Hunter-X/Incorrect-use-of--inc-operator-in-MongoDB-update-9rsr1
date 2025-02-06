# Incorrect use of $inc operator in MongoDB update
This example demonstrates an incorrect use of the `$inc` operator in a MongoDB update operation. The `$inc` operator is used to increment a numerical field by a specified value.  However, in this case, a string ('abc') is provided as the increment value, resulting in an error.

## Bug
The code attempts to increment the 'count' field by 'abc', which is not a valid numerical value.

## Solution
The solution involves using a valid numerical value as an argument for the `$inc` operator. This example replaces the string 'abc' with the number 1.
