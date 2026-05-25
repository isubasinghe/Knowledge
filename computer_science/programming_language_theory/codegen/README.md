# codegen

## Basic idea

The compiler back-end: lowering an intermediate representation to target machine instructions, allocating registers, scheduling, and emitting binary code.

## Key facts

- Common IRs: three-address code, SSA.
- Phases: instruction selection → scheduling → register allocation → emission.
- Register allocation reduces to graph colouring on the interference graph.

