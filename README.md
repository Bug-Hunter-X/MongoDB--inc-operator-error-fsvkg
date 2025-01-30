# MongoDB $inc Operator Error
This example demonstrates an incorrect usage of the MongoDB `$inc` operator.  The `$inc` operator is used to increment a numeric field by a specified value.  However, in this example, a string is used as the increment value, leading to an unexpected result.  The solution shows the correct usage, incrementing the field using a numeric value.

## Bug
The bug lies in the `updateOne` operation.  The `$inc` operator is supplied with a string value ("1") instead of a numeric value (1). This causes MongoDB to either throw an error or produce unexpected results.

## Solution
The solution corrects the `$inc` operator by supplying a numeric value for the increment. This ensures that the counter field is correctly incremented.