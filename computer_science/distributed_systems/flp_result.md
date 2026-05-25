# FLP result

## Basic idea

Fischer-Lynch-Paterson (1985): in an asynchronous message-passing system, no *deterministic* consensus algorithm can guarantee termination if even a single process can crash. Practical systems sidestep it with randomness, failure detectors, or partial synchrony.

## Key facts

- No deterministic protocol solves consensus under async + 1 crash.
- Workarounds: randomised consensus (Ben-Or), partial synchrony (Paxos/Raft with leader-election timeout), unreliable failure detectors (e.g. $\Diamond W$).
- Holds even if the network is reliable — the issue is asynchrony, not faults.

## FLP result
Impossibility of Distributed Consensus with One Faulty Process
The problem of consensus is known to have a solution under a
synchronous network. The FLP result shows that in an asynchronous setting, 
where only one processor might crash, there is no distributed algorithm that solves the 
consensus problem.
