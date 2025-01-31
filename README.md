# Uninitialized Map Access Panic in Go

This repository demonstrates a common error in Go when working with maps: accessing a key in an uninitialized map.  This leads to a runtime panic because the map doesn't exist yet.

## The Bug

The `bug.go` file shows a simple program that attempts to assign a value to a key in an uninitialized map. This results in a panic because the map is nil.

## The Solution

The `bugSolution.go` file shows how to correctly initialize the map before accessing keys.  This prevents the panic.