# Tcl List Index Out of Bounds Error Handling

This repository demonstrates a common error in Tcl when accessing list elements using an index that is out of bounds. The original code lacks robust error handling leading to unexpected crashes.  The solution implements improved error handling to prevent this.

## Bug Description
The `get_element` procedure does not properly handle cases where the provided `index` is out of the valid range for the list.  This results in an error if an attempt is made to access an element beyond the list's boundaries.

## Solution
The improved version adds a check to ensure that the provided index is within the valid range (0 to list length -1). If the index is out of range, it returns a user-friendly error message instead of crashing.