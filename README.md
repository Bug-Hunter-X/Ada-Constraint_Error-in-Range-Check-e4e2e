# Ada Range Check Bug

This repository demonstrates a common error in Ada programming: failing to handle potential out-of-range values correctly, leading to `CONSTRAINT_ERROR` exceptions.

The `Check_Range` function intends to verify if an integer falls within a specific range (10 to 20). However, the `Main` procedure does not include adequate error handling for cases where the input exceeds this range, resulting in a runtime error.

The solution demonstrates how to add robust error handling to prevent such exceptions and how to use the `exception` handler to gracefully handle situations where the range is violated.

## How to reproduce
1. Compile the provided Ada code (bug.ada).
2. Run the compiled program. You should see a `CONSTRAINT_ERROR` exception.

## Solution
The bug is fixed by adding exception handling in the main procedure. See bugSolution.ada for the correction.
