# Cocomo

## Basic idea

COnstructive COst MOdel (Boehm, 1981): an algorithmic cost-estimation model fitted from real project data. Basic COCOMO estimates effort and schedule from KLOC alone; intermediate/detailed variants layer in cost drivers.

## Key formulas

- Basic effort: $E = a \cdot (\text{KLOC})^b$ person-months
- Basic schedule: $D = c \cdot E^d$ months
- **Organic** (small, familiar): $a=2.4,\ b=1.05,\ c=2.5,\ d=0.38$
- **Semi-detached** (medium): $a=3.0,\ b=1.12,\ c=2.5,\ d=0.35$
- **Embedded** (large, strict constraints): $a=3.6,\ b=1.20,\ c=2.5,\ d=0.32$

