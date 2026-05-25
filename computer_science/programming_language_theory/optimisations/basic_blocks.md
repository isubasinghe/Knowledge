# Basic Blocks

## Basic idea

A maximal straight-line sequence of instructions with one entry and one exit: control enters only at the top, exits only at the bottom, no internal branches. The atomic unit of intra-procedural analysis.

## Key facts

- Identified by leaders: first instruction, any branch target, any instruction after a branch.
- Nodes of the control-flow graph (CFG).
- Many optimisations are *local* (within a basic block); global ones use the CFG.

