# Processes and threads

## Basic idea

A process is the OS's unit of resource allocation (address space, open files); a thread is its unit of scheduling. New processes are usually created by *fork* (duplicate) + *exec* (replace image), with copy-on-write avoiding the actual copy.

## Key facts

- `fork()` duplicates address space; pages stay shared and read-only until written (copy-on-write).
- Process creation in distributed OS uses transfer + location policies (where to run).
- Process migration: cheap when code is architecture-independent and resources are migrate-able.

A process encapsulates the basic resources of memory and processor time. It also encapsulates other higher level resources. Each process:

* has an address space and has some amount of allocated memory.
* consists of one or more threads that are given processor timem, including thread sychronization.
* higher level resources such as open file descriptors.

## Creation of a new process

The operating system usually provides a way to create processes. in UNIX the `fork` system call is used to **duplicate** the callers address space, creating a new address space for a new process.

### Copy on write

When a new process is created via `fork`, the address space is copied. The new process code is identical and is usually read-only so that it can be shared in real memory and no actual copying of memory is required. This is fater and more efficient than making a copy. Copy on write is a technique that makes a copy of a memory region only when the new process actually writes to it.

## New processes on distributed systems

In a distributed system there is a choice as to where the new process will be created on. In a distributed operating system, this choice is made by the operating system. The decision is largely a matter of policy and some categories are:

* **transfer policy :** determines whether the new process is allocated locally or remotely. 
* **location policy :** determines which host, from a set of given hosts, the new process should be allocated on.

  The policy is often transparent to the user and will attempt to take into account such things as relative load across hosts, IPC, architectures and specialised resources that processes may require.

## Process migration

Processes can be migrated from one host to another by copying their address space. Depending on the platform and on the resources that are in current use by the process, process migration can be more or less difficult. Process code is often CPU dependant, this obviously introduces heterogenity issues.

