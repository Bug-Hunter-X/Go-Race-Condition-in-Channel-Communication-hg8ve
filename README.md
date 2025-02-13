# Go Race Condition in Channel Communication

This repository demonstrates a common race condition in Go programs involving channel communication.  The program launches multiple goroutines that concurrently attempt to receive data from a single channel. Without proper synchronization, this can lead to unexpected behavior, including incorrect output or deadlocks.

The `bug.go` file contains the erroneous code, highlighting the race condition. The `bugSolution.go` file provides a corrected version that properly handles the synchronization to avoid the race condition.

## How to Run

1. Clone this repository.
2. Navigate to the repository directory.
3. Run the buggy code: `go run bug.go`
4. Run the corrected code: `go run bugSolution.go`

Observe the differences in output and behavior between the two versions.

## Learning Points

This example illustrates the importance of proper synchronization when working with concurrent operations in Go.  Failing to do so can result in subtle and difficult-to-debug issues.