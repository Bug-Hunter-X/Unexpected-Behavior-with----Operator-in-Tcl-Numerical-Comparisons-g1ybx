# Tcl Numerical Comparison Bug

This repository demonstrates a common error in Tcl when using the `==` operator for numerical comparisons.  The `==` operator in Tcl performs string comparison, which can lead to unexpected results if you intend to compare numbers.

## Bug Description
The provided `bug.tcl` file contains a procedure `badproc` that attempts to compare two numbers. However, because it uses `==`, the comparison is done lexicographically (as strings), resulting in incorrect outputs.

## Bug Solution
The solution, found in `bugSolution.tcl`, uses the `expr` command to perform a numerical comparison. This ensures accurate results when comparing numbers in Tcl.

## How to Reproduce
1. Run `bug.tcl`. Observe the incorrect results.
2. Run `bugSolution.tcl`. Observe the correct results.

This example highlights the importance of understanding the nuances of Tcl's operators when working with numerical data.