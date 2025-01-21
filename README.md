# MongoDB $inc Operator Error: Non-numeric Increment Value

This example demonstrates an error that occurs when using MongoDB's `$inc` operator with a non-numeric value.
The `$inc` operator is used to increment a numeric field by a specified value.  If a non-numeric value is provided, the update operation will fail.

## Bug
The provided code attempts to increment the `count` field by the string value 'abc'. This is an incorrect usage of the `$inc` operator and will throw an error.

## Solution
The solution involves ensuring the value being used with the `$inc` operator is a valid number (integer or double).