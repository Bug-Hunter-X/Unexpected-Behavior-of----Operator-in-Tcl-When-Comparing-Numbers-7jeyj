# Tcl == Operator Bug

This repository demonstrates an uncommon bug in Tcl related to the behavior of the `==` operator when comparing numbers.  The `==` operator in Tcl performs string comparison rather than numerical comparison. This can lead to unexpected results when comparing numbers represented as strings and actual numbers.

The `bug.tcl` file shows the problematic code, and `bugSolution.tcl` presents the corrected version.

## How to Reproduce

1.  Clone this repository.
2.  Run `bug.tcl` using a Tcl interpreter.
3.  Observe the unexpected output.
4.  Run `bugSolution.tcl` to see the corrected behavior.

## Solution

The solution involves using the `eq` operator for numerical comparison instead of `==`. The `eq` operator compares the numerical values, avoiding the string comparison issue.