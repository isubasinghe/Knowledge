# Parsing Expression Grammer \(PEG\) parser

## Basic idea

Grammar formalism where each rule is a *deterministic*, prioritised, ordered choice (`/`) rather than the unordered `|` of CFGs. Always unambiguous: the first alternative that matches wins. With memoisation ("Packrat"), parses in linear time.

## Key formulas

- Time (Packrat): $O(n)$, space $O(n)$
- Choice is ordered: $A / B$ tries $A$ first; on success, $B$ is never tried.
- Strictly different power than CFGs — can express $a^n b^n c^n$.

