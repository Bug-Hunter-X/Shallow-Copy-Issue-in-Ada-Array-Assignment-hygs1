# Ada Shallow Copy Bug
This example demonstrates a common pitfall in Ada: shallow copying of arrays.  When an array is assigned to another using the `:=` operator, only the reference is copied.  Modifications to one array will affect the other.

The `bug.ada` file contains code exhibiting this issue. The `bugSolution.ada` file provides a corrected version using array aggregates for deep copy.

This is a critical issue to understand to prevent unexpected program behavior and data corruption.