# Size Estimation

## Basic idea

Estimating *how big* the software will be — a prerequisite for any algorithmic cost model. Three popular metrics: SLOC (post-hoc, language-dependent), Function Points (from requirements), Use Case Points (from use cases).

## Key facts

- SLOC: easy to count after the fact, useless to predict beforehand without analogous projects.
- FP: requires written requirements spec; language-independent.
- UCP: needs well-written use cases.

Commonly used metric for software size estimation

* Source lines of code \(SLOC\)
* Function Points \(FP\)
  * Based on Requirement specs
* Use case points \(UCP\)
  * Based on Use Cases

## Source Lines of Code \(SLOC\)

There are two types of SLOC:

* Physicial SLOC: Count excluding comments and blank lines.
* Logical SLOC: Measure the number of executable "statements", but their specific definitions are tied to specific computer languages. 

### Advantages of SLOC

* Scope for Automation of counting: since lines of code is a physical entity it is easy to count and can be automated using a tool. 
* An intuitive metric: Lines of code serves as an intuitive metric for measuring the size of software because it can be seen and the effect of it can be visualized. 

### Disadvantages of SLOC

* Variability: depends on programmer experience, language, framework support, reuse etc.
* It is difficult to estimate the number of lines of code that will be needed to develop a system from information that is available in analysis and design phases
* Lack of universally accepted definition for exactly what a line of code is. 

