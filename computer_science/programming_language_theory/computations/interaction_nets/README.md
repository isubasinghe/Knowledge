# Interaction Nets

## Basic idea

A graph-rewriting model of computation due to Lafont (1990). A net is built from agents (nodes) with ports; a fixed set of *interaction rules* rewrites pairs of connected agents. Confluent, local, and inherently parallel — the basis of optimal $\lambda$-calculus reducers (e.g. HVM).

## Key facts

- Each agent has one *principal port* and several auxiliary ports; rules fire only on principal-principal connections.
- Strong confluence: any two reductions of the same redex give the same result (Church-Rosser holds trivially).
- Cost model: number of interactions (β-reductions for $\lambda$ encodings).
