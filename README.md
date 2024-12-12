# VHDL Counter Overflow Bug

This repository demonstrates a common error in VHDL code: an integer overflow in a counter.

## Bug Description
The `buggy_counter.vhdl` file contains a counter that is intended to count from 0 to 15. However, there is a potential overflow issue when the counter reaches 15. The solution addresses this with proper range handling.

## How to Reproduce
1. Simulate `buggy_counter.vhdl` using a VHDL simulator (e.g., ModelSim, GHDL).
2. Observe the counter's behavior after it reaches the maximum value (15).

## Solution
The `fixed_counter.vhdl` file provides a corrected version of the counter, addressing the overflow issue.  It uses a modulo operation to ensure that the counter wraps around correctly.

## Learning Points
* Careful consideration of data types and range constraints is crucial when designing counters and other numerical components in VHDL.  A simple integer type, while intuitive, can lead to unwanted overflow.