# Function Points

## Basic idea

Measure software size by the *functionality* delivered to the user, not by code volume. Counts inputs, outputs, inquiries, internal files, and external interfaces; multiplies by complexity weights; adjusts by 14 general system characteristics.

## Key formulas

- Adjusted FP: $FP = UFP \times VAF$
- VAF: $VAF = 0.65 + 0.01 \sum_{i=1}^{14} F_i$, with each $F_i \in [0,5]$
- $UFP = \sum_{\text{type, complexity}} (\text{count} \times \text{weight})$

Is used to express the amount of functionality in a software system, as seen by the user. A higher number of function points indicates more functionality. Typically used to:

* Estimate the cost and effort required to design, code and test a software system.
* Predict the number of errors
* Predict the number of components
* Measure productivity

  Function Points are computed from the Software Requirements Specification \(SRS\)

## Advantages of function points

* Measure the size of the solution instead of the size of the problem 
* Requirements are the only thing needed for function points count
* Can be estimated early in analysis and design 
* Is independant of technology 
* Is independant of programming languages

## Disadvantages of function points

* A well defined requirements specification is necessary
* Gaining proficency is not easy, the learning curve is quite long
* Could be quite time-consuming this could be costly

