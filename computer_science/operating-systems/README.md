# Operating Systems 

## Basic idea

The software layer between hardware and applications. Manages CPU scheduling, memory, I/O, files, and security; provides processes/threads, an address-space abstraction, and system calls.

## Key facts

- Core abstractions: processes, threads, virtual memory, files, sockets.
- Scheduling: preemptive (round-robin, CFS), priority, real-time.
- Memory hierarchy: registers → L1/L2/L3 cache → RAM → disk; each $\sim 10\times$ slower than previous.
- Modes: user / kernel; syscalls cross the boundary.

## Resources 
  * http://littleosbook.github.io/
