# Case-Sensitive String Comparison in Tcl

This repository demonstrates a common, yet subtle, error in Tcl: case-sensitive string comparison.  The `badproc` procedure incorrectly uses `==` which performs case-sensitive comparisons.  The solution showcases the use of `string compare` to achieve case-insensitive comparisons.

## Bug

The `bug.tcl` file contains a procedure that demonstrates the issue.  It returns 1 if two strings are identical, and 0 otherwise, but fails if only the casing is different. 

## Solution

The `bugSolution.tcl` file provides a corrected procedure using `string compare`. This version correctly handles case-insensitive string comparisons.

## Usage

1. Clone the repository.
2. Run the `bug.tcl` script to observe the erroneous behavior.
3. Run the `bugSolution.tcl` script to see the correct implementation.