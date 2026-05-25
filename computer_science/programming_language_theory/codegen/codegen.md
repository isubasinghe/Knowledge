# Codegen

## Basic idea

Translation from an intermediate representation to executable target code. The three classical sub-problems: instruction selection (which target ops?), register allocation (which value lives where?), instruction scheduling (in what order?).

## Key facts

- Instruction selection: tiling the IR DAG with target patterns (BURS, maximal munch).
- Register allocation: graph colouring on the interference graph — NP-hard; Chaitin / Briggs / linear-scan heuristics.
- Scheduling: list scheduling, software pipelining, trace scheduling.

