# parsers

## Basic idea

Map a token stream to a parse tree according to a grammar. Classes of parsers trade expressive power for efficiency: LL ⊂ LALR ⊂ LR ⊂ CFG ⊂ PEG (incomparable but practical).

## Key facts

- LL(1), LR(0/1), SLR(1), LALR(1): all $O(n)$ table-driven.
- Earley: any CFG, $O(n^3)$ worst case / $O(n^2)$ unambiguous / $O(n)$ deterministic.
- PEG: deterministic, $O(n)$ with memoisation (Packrat); no ambiguity (longest match wins).

