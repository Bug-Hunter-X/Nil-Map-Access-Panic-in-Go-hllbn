# Go Nil Map Access Panic

This repository demonstrates a common error in Go programs: panics due to accessing elements of a nil map.  Direct access to an uninitialized map will result in a runtime panic, crashing the program.  Proper error handling and nil checks are crucial to prevent this.

## Bug
The `bug.go` file contains a simple Go program that demonstrates the problem.  It attempts to assign a value to a map without first initializing it, causing a panic.

## Solution
The `bugSolution.go` file shows the corrected version. Before accessing the map, it checks for nil and initializes it if necessary.