# distributed\_systems

## Basic idea

Multiple networked nodes that coordinate to appear as one system. The interesting problems all come from partial failure, asynchrony, and the absence of a global clock.

## Key formulas

- CAP: under partition, choose either consistency or availability
- FLP: no deterministic consensus in async with even one crash failure
- Quorum: $R + W > N$ ⇒ read sees most recent write
- $f$-Byzantine consensus needs $N \ge 3f+1$ nodes

