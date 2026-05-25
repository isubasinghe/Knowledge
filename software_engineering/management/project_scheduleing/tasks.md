# Tasks

## Basic idea

Tasks are either *unconstrained* (start anytime) or *constrained* (depend on another task). Four kinds of dependency, named by which endpoints connect: finish-to-start (most common), start-to-start, finish-to-finish, start-to-finish (rare).

## Key facts

- Finish-to-Start (FS): predecessor finishes → successor starts. Default.
- Start-to-Start (SS): successor can't start until predecessor starts.
- Finish-to-Finish (FF): successor can't finish until predecessor finishes.
- Start-to-Finish (SF): rare, used for handover scheduling.

## Tasks

### Identifying task dependencies

Tasks can be

- **Unconstrained:** The task can start at any time
- **Constrained:** The task depends on another task

### Type of task dependencies

| Dependancy       | Description                                         | Representation |
| ---------------- | --------------------------------------------------- | -------------- |
| Finish-to-Start  | Predecessor must finish before successor may start  |                |
| Start-to-Start   | Predecessor must start before successor may start   |                |
| Finish-to-Finish | Predecessor must finish before successor may finish |                |
| Start-to-Finish  | Predecessor must start before sucessor may finish   |                |
