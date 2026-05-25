# Effort-time estimation

## Basic idea

Estimate the *effort* (work) and *time* (duration) for each task. The two are not interchangeable — Brooks's mythical man-month: adding people to a late project makes it later.

## Key formulas

- PERT three-point: $T_E = (O + 4M + P)/6$
- PERT std dev: $\sigma = (P - O)/6$
- COCOMO schedule from effort: $T_{dev} = 2.5 \cdot E^{0.38}$ months (organic)

## Effort-time estimation

A common measure for estimating the effort for software is **man-months**

### The mythical man-month

- man-months is a misleading measure to estimate software.
- adding people to a project that is behind schedule could result in more damage than helping it.

### Time Estimation

- optimistic time _O_
- pessimistic time _P_
- most likely time _M_
- expected time _TE_

TE = ( _O_ + 4\*_M_ + _P_)/6
