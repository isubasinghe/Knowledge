# Cocomo

## Basic idea

COnstructive COst MOdel (Boehm, 1981). An algorithmic cost-estimation model fitted from real project data. Basic COCOMO estimates effort and schedule from size in KLOC; intermediate / detailed variants layer in cost drivers.

## Key formulas

- Effort: $E = a \cdot (\text{KLOC})^b$ person-months
- Schedule: $D = c \cdot E^d$ months
- **Organic**:        $a=2.4,\ b=1.05,\ c=2.5,\ d=0.38$
- **Semi-detached**:  $a=3.0,\ b=1.12,\ c=2.5,\ d=0.35$
- **Embedded**:       $a=3.6,\ b=1.20,\ c=2.5,\ d=0.32$

## Cocomo

Derived from collecting data from a large number of software projects and deriving formulae that best fits the observations
