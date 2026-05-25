# Definitions

## Basic idea

Core vocabulary for scheduling: *activity* (work taking time + resources), *milestone* (zero-duration checkpoint), *float* (slack — how much an activity can slip), *critical path* (longest activity chain — slack = 0).

## Key formulas

- $\text{Total float} = LS - ES = LF - EF$
- $\text{Free float} = \min(ES_{succ}) - EF$
- Critical activity: $\text{total float} = 0$
- Critical path: any path of critical activities from start → end.

## Definitions

### Activity (Task)

Is a part of the project that requires resources and time

### Milestone

Is the completion of an activity that provides evidence of a deliverable completion or end of a phase - is an event that takes zero time.

### Free float (Free slack)

Is the amount of time that a task can be delayed without causing a delay to subsequent tasks

### Total float (total slack)

Is the amount of time that a task can be delayed without delaying project completion

### Critical path

Is the longest continuous path taken from the initial event to the terminal event

### Critical activity

Is an activity where total slack is zero
