# VHDL Counter Reset Bug

This repository demonstrates a potential off-by-one error in a simple VHDL counter's reset condition.  The `buggy_counter.vhdl` file contains the buggy code.  The `fixed_counter.vhdl` file provides the corrected version.

## The Bug
The issue lies in the reset condition within the counter's process.  Under certain circumstances, the counter might not correctly reset to 0.

## The Solution
The solution involves ensuring the reset condition properly sets the internal counter to 0.  This has been corrected in `fixed_counter.vhdl`

## How to Reproduce
1. Simulate the `buggy_counter.vhdl` using your preferred VHDL simulator.
2. Observe the counter's behavior, particularly when the reset signal (`rst`) is asserted and deasserted.
3. Compare the output with the expected behavior to identify the error.
4. Simulate the `fixed_counter.vhdl` to see the corrected output.
