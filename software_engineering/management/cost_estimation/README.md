# cost\_estimation

## Basic idea

Predicting effort, schedule, and cost of a software project. Approaches range from expert judgement and analogy to algorithmic models (COCOMO, function points, use-case points).

## Key formulas

- General algorithmic: $\text{Effort} = A \cdot \text{Size}^B \cdot M$
- COCOMO basic: $E = a (\text{KLOC})^b$
- PERT three-point: $e = (o + 4m + p)/6$
- Function points: $FP = UFP \times VAF$, $VAF = 0.65 + 0.01 \sum_{i=1}^{14} F_i$

