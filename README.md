# F# Mutable Variable Swap Bug

This repository demonstrates a common pitfall when working with mutable variables in F#. The `swap` function, intended to exchange the values of two mutable variables, unexpectedly modifies the original variables due to pass-by-reference semantics.

## Bug Description

The `bug.fs` file contains code that attempts to swap two integer variables using a `swap` function.  However, due to F#'s pass-by-reference behavior for mutable variables, the output is not as expected, leading to an unexpected result. 

## Solution

The `bugSolution.fs` file provides a corrected version of the code. It creates a new tuple with the swapped values. This correctly swaps the variable values without modifying the original ones.