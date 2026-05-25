# SSA form

## Basic idea

In LLVM IR every register is assigned exactly once. To represent values that depend on which control-flow predecessor was taken, LLVM uses `phi` instructions at the start of basic blocks.

## Key formulas

- $\phi$-function: `%x = phi i32 [%a, %bb1], [%b, %bb2]`
- Dominance frontier $DF(B)$: where $\phi$-nodes are inserted.

See [SSA](../../../computer_science/programming_language_theory/codegen/single_static_assignment_form.md) LLVM does not allow multiple assignments to registers

LLVM offers the phi function to choose between values.

